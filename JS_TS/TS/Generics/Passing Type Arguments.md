https://www.typescriptlang.org/docs/handbook/2/generics.html#handbook-content

# Returning Multiple Generics

When it comes to generics the way TS treats 1 vs multiple generics differs in how it infers the types:

```ts
const returnBothOfWhatIPassIn = <A>(a: A) => {
  return a
};

const result = returnBothOfWhatIPassIn("a");

// const result: "a"
```

In the above example we are simply returning what we pass in. The type that is returned is actually going to be `"a"`.

However when we move to multiple:

```ts
const returnBothOfWhatIPassIn = <A, B>(a: A, b: B) => {
  return {
    a,
    b,
  };
};

const result = returnBothOfWhatIPassIn("a", 1);

//const result: {  
//	a: string;  
//	b: number;  
//}
```

We can see that it actually returns their types. If we wanted the exacts of what was passed it to be returned as types we can do:

```ts
const returnBothOfWhatIPassIn = <A extends string, B extends number>(a: A, b: B) => {
  return {
    a,
    b,
  };
};

const result = returnBothOfWhatIPassIn("a", 1);

//const result: {  
//	a: "a";  
//	b: 1;  
//}
```

## Typing Object Parameters

```ts
const returnBothOfWhatIPassIn = <T1, T2>(params: { a: T1; b: T2 }) => {
  return {
    first: params.a,
    second: params.b,
  };
};

const result = returnBothOfWhatIPassIn("a", 1);

//const result: {  
//	a: string;  
//	b: number;  
//}
```

Similar to the previous approach we can use the same syntax to infer the types of `a and b`. We do not actually have to extend the same object we are passing in. What we are doing in the above is we are saying there are going to be 2 values I want you to infer. These are where the slots lie for you to do so.

# Generics in Classes

# Passing Type Arguments and Inference

Passing generic to a function is quite straight forward:

```ts
export const createSet = <T>() => {
  return new Set();
};
```

This allows you to then tell the type and it will be able to infer the return:

```ts
const stringSet = createSet<string>(); // Set<string>
const numberSet = createSet<number>(); // Set<number>
```

However you can also modify the above as follows:

```ts
export const createSet = <T>(initialValue?: T) => {
  return new Set<T>();
}
```

This means you pass your types as:

```ts
const stringSet = createSet('123'); // Set<string>
const numberSet = createSet(456); // Set<number>
```

This is the same result but rather than explicit in what you are passing as a type argument. You use a argument for the function to infer.

# Default Generic

Similar to defaults in normal JS/TS you can create generic defaults:

```ts
export const createSet = <T = string>() => {
  return new Set<T>();
}
```

# Infer Types from Generic Type Arguments

You can use generics to infer props. This becomes very useful for easily extending functionality and inferring the values on return:

```ts
export class Component<TProps> {
  private props: TProps;

  constructor(props: TProps) {
    this.props = props;
  }

  getProps = () => this.props;
}

const cloneComponent = <TProps>(component: Component<TProps>): Component<TProps> => {
  return new Component(component.getProps());
};
```

In the example above we have a class component that expects a generic TProps. We can use this to our advantage. By expecting the component to be passed in we can infer the `TProps` value. This means we can then say when returning it is going to give us the output with the passed properties.

This inference is powerful as you can now simplify this more:

```ts
const cloneComponent = <TProps>(component: Component<TProps>) => {
  return new Component(component.getProps());
};
```

Which will infer the same.


