
## Utility Types

Typescript provides several [utility types](https://www.typescriptlang.org/docs/handbook/utility-types.html#awaitedtype) to facilitate common type transformations. These utilities are available globally.

These are useful for inference and extracting types.

## Keyof

If you are wanting to extract the keys of an object or a type you need to make use of the `keyof` keyword.

```ts
type TestingFrameworks = {
	a: string;
	b: string;
	c: string;
};

type TestingFramework = keyof TestingFrameworks;
// a | b | c
```

The above takes our *TestFrameworks* type which has keys `a,b,c` and then using `keyof` we then create a union of those keys.

If we wanted to get the keys of a object we first need to create a type using `typeof` and then use the `keyof`:

```ts
const testingFrameworks = {
	a: 'a';
	b: 'b';
	c: 'c';
};

type TestingFramework = keyof typeof testingFrameworks;
// a | b | c
```

