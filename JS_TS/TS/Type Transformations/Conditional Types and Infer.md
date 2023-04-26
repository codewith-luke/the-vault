https://www.typescriptlang.org/docs/handbook/2/conditional-types.html
https://www.typescriptlang.org/docs/handbook/2/conditional-types.html#inferring-within-conditional-types

## Infer 

Infer is basically casting the type to a 'variable' that we call whatever we want and can then use it as we see fit:

```ts
type GetDataValue<T> = T extends { data: infer TData }
  ? TData
  : never;
```

## Infer Generics

Sometimes you may have an interface that has some generic properties that you may want to infer the value from.

```ts
type GetPoint<T> = T extends MyComplexInterface<any, any, any, infer TPoint>
  ? TPoint
  : never;
```

This would then extract the type we care about and return it's type. You could infer one or multiple.

## Extract parts of a string

Sometimes you may want to extract aspects of a string or value and using infer can allow you to do this: 
```ts
type GetSurname<T> = T extends `${infer First} ${infer Last}` ? Last : never 
```

## Extract the Result of an Async Function

With the below code we are saying that we are expecting a function which returns a Promise. This is done using `extends`. We can then infer the return type of the Promise. In the below case we are getting a specific property within the Promise reponse called `props`: 

```ts
type InferPropsFromServerSideFunction<T> = T extends () => Promise<{
  props: infer P
}>
  ? P
  : never
```

## Two Methods for Extracting the Result of Multiple Possible Functions

There may be scenarios where you need to extract the return type during multiple scenarios. One may be you have a function that can take an object or function to do some form of work. 

The one option of doing this is going over each possibility and using the ternary operator to do so:

```ts
type GetParserResult<T> = T extends {
  parse: () => infer TResult
}
  ? TResult
  : T extends () => infer TResult
  ? TResult
  : T extends {
      extract: () => infer TResult
    }
  ? TResult
  : never
```

The above example has each possible scenario where we extract the desired restult from those scenarios. We can clean this up with a `union`:

```ts
type GetParserResult<T> = T extends
  | {
      parse: () => infer TResult
    }
  | {
      extract: () => infer TResult
    }
  | (() => infer TResult)
  ? TResult
  : never
```

Here we are simply creating each scenario as a union. If you type extends one of those possibilities we then have catered for the typer extraction and then use the ternary and infer to retrieve. 

## Using Generic Context to avoid Distributive Conditional Types

https://www.typescriptlang.org/docs/handbook/2/conditional-types.html#distributive-conditional-types

When it comes to conditional types there is a difference between a union type that is expressed as a type and on that is via a generic. When conditional types act on a generic type, they become distributive when given a union type. Think of it like iteration over all possibilities.

There are two ways to get around this:

```ts
type Fruit = "apple" | "banana" | "orange"

type GetAppleOrBanana<T> = T extends "apple" | "banana" ? T : never

type AppleOrBanana = GetAppleOrBanana<Fruit>
```

This works as we are pulling out union of Fruit into a generic T. The members of the union distribute acorss it. In other words, T will become each individual member of the union, and the conditional type will iterate over each one. Where if we look at something like:

```ts
type AppleOrBanana = Fruit extends "apple" | "banana" ? Fruit : never
```

What we are actually doing is checking an exact match on the union itself.

There is also another solution of:

```ts
type AppleOrBanana = Fruit extends infer T
  ? T extends "apple" | "banana"
    ? T
    : never
  : never
```

Here we create our generic of our union using `extends infer T` in order to create the same scenario as in first solution.

