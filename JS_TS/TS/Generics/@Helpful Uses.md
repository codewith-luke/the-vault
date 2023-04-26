
# Strongly Typed Reduce

```ts
const obj = array.reduce<Record<string, { name: string }>>((accum, item) => {
  accum[item.name] = item;
  return accum;
}, {});
```

# Generics in Class Name Creator

```ts
/**
The below infers that each key of the record will be of type string and is stored in a generic `TVariant`. This then means that we can use this generic in the `type` argument and ensure all the others is a string array. 
*/

const createClassNamesFactory =
  <TVariant extends string>(classes: Record<TVariant, string>) =>
  (type: TVariant, ...otherClasses: string[]) => {
    const classList = [classes[type], ...otherClasses];
    return classList.join(" ");
  };
```

# A Function with a Dynamic Number of Arguments

The below pattern is useful for determining the type passed in and then inferring the expected types that the function would need.

```ts
interface Events {
  click: {
    x: number;
    y: number;
  };
  focus: undefined;
}

export const sendEvent = <TEventKey extends keyof Events>(
  event: TEventKey,
  ...args: Events[TEventKey] extends undefined
    ? []
    : [payload: Events[TEventKey]]
) => {
  // Send the event somewhere!
};
```

The following code is doing a lot so let's break it down:

1) First we are creating a generic to check the key value passed in is of one of the Events interface. So `click` or `focus`
2) With args we then go and infer or check if the passed in args which map to `click | focus` extends undefined
3) If it is undefined we return and empty array
4) Otherwise return the payload which is the the RHS of the event. So if it was `click` it would return the `x:number y: number`.

# Extracting Object Properties with Generics

This is another somewhat complex problem. The use case behind it would be that we pass in a specific object, tell the function that we only care about certain properties in it and want good type detection. So let's break it down:

```ts
const pick = <TObj, TPicked extends keyof TObj>(
  obj: TObj,
  picked: Array<TPicked>
) => {
  return picked.reduce((acc, key) => {
    acc[key] = obj[key];
    return acc;
  }, {} as Pick<TObj, TPicked>);
};
```

1) First we define `TObj` and `TPicked`. Picked being the properties of `TObj` that we care about. We then extend and get all the keys of `TObj`. So if we passed an object of `{a: 1: b: 2}` then `TPicked` would infer the values passed in as an Array. So if we passed `["a"]` then picked would be made up of `a`.
2) We then cast the original object in the reduce and make use of the `Pick` utility function and give it the keys we want it to pick from and the base object `TObj`.

# Type Form Validation

There may be scenarios where we have functions that return functions that return functions. In the below scenario is a form validator that that expects some validator functions, which will then return you a function to pass in data that would then run through those initial validator functions.

The part that we want out of this is when we pass our validator functions to `makeFormValidatorFactory` and then the things we want to validate `createFormValidator` we want to ensure that when we extend these things that types are returned accurately.

```ts
 const makeFormValidatorFactory =
  <TValidatorKeys extends string>(
    validators: Record<TValidatorKeys, (value: string) => string | void>
  ) =>
  <TObjKeys extends string>(
    config: Record<TObjKeys, Array<TValidatorKeys>>
  ) => {
    return (values: Record<TObjKeys, string>) => {
      const errors = {} as Record<TObjKeys, string | undefined>;

      for (const key in config) {
        for (const validator of config[key]) {
          const error = validators[validator](values[key]);
          if (error) {
            errors[key] = error;
            break;
          }
        }
      }

      return errors;
    };
  };

const createFormValidator = makeFormValidatorFactory({
  required: (value) => {
    if (value === "") {
      return "Required";
    }
  },
  minLength: (value) => {
    if (value.length < 5) {
      return "Minimum length is 5";
    }
  },
  email: (value) => {
    if (!value.includes("@")) {
      return "Invalid email";
    }
  },
});

const validateUser = createFormValidator({
  id: ["required"],
  username: ["required", "minLength"],
  email: ["required", "email"],
});

```

1) First we get each key from the passed in validator function object
2) We hand that over to the `validators` as a type `Record` that would contain the different function return signatures
3) When `makeFormValidatorFactory` returns `createFormValidator` we then do the same thing where we only care about the object passed in and its keys to then create the `config` object as a `Record` with the expected structure.
4) We then have the final function which expects a `values: Record<TObjKeys, string>`. This has to be based off the original `createFormValidator` object so we use `TObjeKeys`.
5) Finally we return errors as a `Record` as we build this up as it validates.

# Extracting Types from Strings

The below takes from an example of creating internationalization and checking arguments in a string and enforcing that they be passed in. The first 2 types are helper functions that basically check if a string matches the patter `{something}` and if it does it will extract all of them as either a string or union.

The `translate` function is where it gets more complicated:

```ts
type GetParamKeys<TTranslation extends string> = TTranslation extends ""
  ? []
  : TTranslation extends `${string}{${infer Param}}${infer Tail}`
  ? [Param, ...GetParamKeys<Tail>]
  : [];

type GetParamKeysAsUnion<TTranslation extends string> =
  GetParamKeys<TTranslation>[number];

const translate = <
  TTranslations extends Record<string, string>,
  TKey extends keyof TTranslations,
  TDynamicKeys = GetParamKeysAsUnion<TTranslations[TKey]>
>(
  translations: TTranslations,
  key: TKey,
  ...args: TDynamicKeys extends string
    ? [dynamicArgs: Record<TDynamicKeys, string>]
    : []
) => {
  const translation = translations[key];
  const params: any = args[0] || {};

  return translation.replace(/{(\w+)}/g, (_, key) => params[key]);
};

const translations = {
  title: "Hello, {name}!",
  subtitle: "You have {count} unread messages.",
  button: "Click me!",
} as const;

const buttonText = translate(translations, "button");
```

1) First we are saying that we expect translations to be passed in `as a const`. We then check that it is a record of string.
2) Now that we have this we create the `TKey` and this extends all of our translation keys and can only be one of those.
3) We then have `TDynamicKeys`. This uses our helper function. Where we pass in the select key and extract our params that would be required for it.
4) This DynamicKeys type argument is great as it means we can re-use it at the type level. You will notice it is a default param, not something that will actually be passed in.
5) We then use the `TDynamicKeys` and check that it extends `string`
6) If it does we then say that we will return a union type. The reason for this is out `...args` are spread so that means we need to ensure that we are spreading our arguments across as a `Record`
7) Otherwise return an empty array