Function overloads can be considered somewhat unsafe. This is due to the signature (part where logic happens) being somewhat loose in respecting types. It is therefore recommended to always return the types available in the signature return and this will help the overloads.


# Overloads and Conditionals

Conditionals can turn into quite ugly looking statements and may be better to use something like an overload in order to determine a code path. This can look something like:

```ts
function youSayGoodbyeISayHello(greeting: "goodbye"): "hello";
function youSayGoodbyeISayHello(greeting: "hello"): "goodbye";
function youSayGoodbyeISayHello(
  greeting: "goodbye" | "hello"
): "goodbye" | "hello" {
  return greeting === "goodbye" ? "hello" : "goodbye";
}
```

So you can see here we have our signature where we are declaring all the possible return types. Then we have our overloads that then narrow down these conditions.

# Typing Different Function Use Cases

There may come different scenarios where you want to enforce the type based on how the function is called. So in the below example what we have done is saying that if you are going to pass a number to his function it has to be of `type = 1`. 

```ts
function returnWhatIPassInExceptFor1(t: 1): 2;
function returnWhatIPassInExceptFor1<T extends string>(t: T): T;
function returnWhatIPassInExceptFor1(t: string | 1): unknown {
  if (t === 1) {
    return 2;
  }
  return t;
}
```

This means that if we had to call:

```ts
const resuslt = returnWhatIPassInExceptFor1(3);
```

We would in fact get an error as we have constrained our overloads to only accept a generic that extends a string or a number 1.

# Split Functions into Two Different Call Signatures

This is the original function call. It essentially has 2 paths. One that returns T and one that returns undefined. It would only return undefined if there is no initial data. However if we want our return types to be more accurate we need to provide it different call signatures based on what would happen.
```ts
function useData<T>(params: { fetchData: () => Promise<T>; initialData?: T }): {
  getData: () => T | undefined;
} {
  let data = params.initialData;

  params.fetchData().then((d) => {
    data = d;
  });

  return {
    getData: () => data,
  };
}
```

The below code would achieve this. By creating 2 overrides. One where it has no initial data and returns it's response. Then the one with initial data and its return type. Then the base case that contains it all.

```ts
function useData<T>(params: { fetchData: () => Promise<T> }): {
  getData: () => T | undefined;
};
function useData<T>(params: { fetchData: () => Promise<T>; initialData: T }): {
  getData: () => T;
};
function useData<T>(params: { fetchData: () => Promise<T>; initialData?: T }): {
  getData: () => T | undefined;
} {
  let data = params.initialData;

  params.fetchData().then((d) => {
    data = d;
  });

  return {
    getData: () => data,
  };
}
```

# Handling Default Arguments with Function Overloads

There are times when you can have multiple return types and sometimes you may make use of default arguments. To account for this as per previous code you have to first ensure that your base case accounts for your default (defaults can only be in a base case). You then ensure that your overloads are able to then account for each scenario.

```ts
const obj = {
  a: 1,
  b: 2,
  c: 3,
} as const;

type ObjKey = keyof typeof obj;

function getObjValue(): typeof obj["a"];
function getObjValue<TKey extends ObjKey>(key: TKey): typeof obj[TKey];
function getObjValue(key: ObjKey = "a") {
  return obj[key];
}

const one = getObjValue("a");
const oneByDefault = getObjValue();
const two = getObjValue("b");
const three = getObjValue("c");
```