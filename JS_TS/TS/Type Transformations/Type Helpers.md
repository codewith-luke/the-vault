## Using Constraints to Limit Type Parameters

If you want your generic value to be constrained to a type (which can be important when you are wanting to working with things like string template), you can use the `extends` keyword to then define the type that the generic can be a part of.

```ts
type AddRoutePrefix<TRoute extends string> = `/${TRoute}`;
```

## Function Constraints

There are cases where you may have a function and want to extract the types out of that function such as its return and parameters:

```ts
type GetParametersAndReturnType<T extends (...args: any) => any> = {}
```

Something like the above mimics utilities such as Parameters or Return Type. What we are concerned about is not so much what is passed in, the `extends` aspect is just essentially saying we want to constrain this to a function with any type of args and return and then we can infer these values later on.

## Not Null or Undefined

Typescript does constructional comparisons when checking if things are assignable to each other. You can therefore do the following:

```ts
export type Maybe<T extends {}> = T | null | undefined;
```

This will now check do constructional comparisons on anything other than null and undefined as these do not meet the same makeup of an object. Where strings and the like do. Everything else besides those are objects.

## Non Empty Array

A way to validate that there are at minimum amount of a certain type is by the following:

```ts
type NonEmptyArray<T> = [T, ...Array<T>]; 
```

What this is saying that `NonEmptyArray` expects a type `T` and that it is going to be an array. However the first index of that array we put `T` to say that it must exist. Then we use `...Array<T>` which means that any more elements after is fine they just must be of type T.

```ts
type NonEmptyArray<T> = [T, T, ...Array<T>]; 
```

Doing something like this now means we must then have a min of 2 and so on.

