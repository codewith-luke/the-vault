# Generics with Conditional Types

```ts
function youSayGoodbyeISayHello<TGreeting extends "hello" | "goodbye">(greeting:TGreeting): TGreeting extends "hello" ? "goodbye" : "hello" {
	return (greeting === "goodbye" ? "hello" : "goodbye") as any;
}
```

In the above we are first creating our options for our generic to start `TGreeting extends "hello" | "goodbye"` We then are able to use that generic in our arguments and then finally check which one of our options it extends. 

You will need to wrap it is an `as any` to help Typescript or you would need to cast it to the type it should be expected to be. Essentially telling TS you know better here what should be returned.

# Generic Function Currying

```ts
export const curryFunction =
  <T>(t: T) =>
  <U>(u: U) =>
  <V>(v: V) => {
    return {
      t,
      u,
      v,
    };
  };
  
  const result = curryFunction(1)(2)(3);
```

What we are doing with the above is just taking the type of each function and putting the generic where it is appropriate as if we were calling it directly.


