These types of functions are great for setting up types and really ensuring that we specify the types that we want. They do not really contain logic. They are just helping us define our types better.

# Narrowing at generic level

This function allows you to create narrowing at the generic level:
https://github.com/millsp/ts-toolbelt/blob/319e551/sources/Function/Narrow.ts#L32

In Typescript 5 you can do this with `<const T>...` at the generic.

# Specifying where inference should not happen

https://github.com/millsp/ts-toolbelt/blob/master/sources/Function/NoInfer.ts

# Inference with Identity Functions

In this example we have create our identity function `makeConfigObj`. It's responsibility is to take in what we give it and give us stronger types. So here we are making our routes the generic we want to type from. We check that it extends string and pass them to `ConfigObj`. This then takes those inferred routes and then types our expected return type of `ConfigObj`.

```ts
interface ConfigObj<TRoute extends string> {
  routes: TRoute[];
  fetchers: {
    [K in TRoute]?: () => any;
  };
}

const makeConfigObj = <TRoute extends string>(config: ConfigObj<TRoute>) =>
  config;

export const configObj = makeConfigObj({
  routes: ["/", "/about", "/contact"],
  fetchers: {
    // @ts-expect-error
    "/does-not-exist": () => {
      return {};
    },
  },
});
```

# Reverse Mapped Types

https://www.totaltypescript.com/workshops/type-transformations/mapped-types/map-over-a-union-to-create-an-object

In the below example we create a `makeEventHandlers` identity function. That takes what we pass in and returns it. However what we do with the obj is ensure that it confirms to our `ObjType`

```ts
type ObjType<TObj> = {
  [TKey in keyof TObj]: (value: TKey) => void
}

export function makeEventHandlers<TObj>(obj: ObjType<TObj>) {
  return obj;
}
```

# Narrow with an Array

```ts
interface Fruit {
  name: string;
  price: number;
}

// 1) First we extend an array `Fruit[]` which we
// then use F.Narrow to narrow the types to their literals
export const wrapFruit = <TFruits extends Fruit[]>(
  fruits: F.Narrow<TFruits>
) => {
					// 2) We then get all the possible names from our fruits
					//    array
  const getFruit = <TName extends TFruits[number]["name"]>(name: TName) => {
  
    return fruits.find((fruit) => fruit.name === name) as Extract<
      TFruits[number],
      { name: TName }
    >; // 3) Then because we know what is actully happening here we 
	   //    tell typescript that it will return a specific fruit from
	   //    the array using the Extract util.
  };

  return {
    getFruit,
  };
};
```