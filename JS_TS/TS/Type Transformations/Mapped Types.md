Overviewhttps://www.typescriptlang.org/docs/handbook/2/mapped-types.html

## Selective Remapping
There may be instances where you want to create a new type with only specific keys. You can use the `as` keyword with mappings in conjunction with `extends` to test for your scenario and return `never` when that scenario is not met.

This technique lets us restrict the keys which are mapped back into the object, while still keeping hold of K to index into the object.

```ts
type OnlyIdKeys<T> = {
  [K in keyof T as K extends SearchForId ? K : never]: T[K]
}
```

## Mapping Discriminated Union to an Object

This example below can be useful if you are wanting to first to create a key from a `discriminated union`, in this case *route* and then extract a specifc key within that discriminated union as the new type.

```ts
type Route =
  | {
      route: "/";
      search: {
        page: string;
        perPage: string;
      };
    }
  | { route: "/about"; search: {} }
  | { route: "/admin"; search: {} }
  | { route: "/admin/users"; search: {} };

type RoutesObject = {
  [R in Route["route"]]: Extract<Route, { route: R }>["search"]
}
```

You can also achieve the above with:

```ts
type RoutesObject = {
  [R in Route as R["route"]]: R["search"]
}
```

## Mapping an Object to Union

Sometimes we may want to take an interface or an object and turn that into a specific type of union. In the example below we are taking `Values` and creating a union of tuples. 

This is done by first creating the structure we want and then using `[keyof Values]` to essentially say for every key of Values we want to do the following and put that into a union.

```ts
interface Values {
  email: string;
  firstName: string;
  lastName: string;
}

type ValuesAsUnionOfTuples = {
  [V in keyof Values]: [V, Values[V]];
}[keyof Values];

type tests = [
  Expect<
    Equal<
      ValuesAsUnionOfTuples,
      ["email", string] | ["firstName", string] | ["lastName", string]
    >
  >,
];
```

## Discriminated Union into a Union

```ts
type Fruit =
  | {
      name: "apple";
      color: "red";
    }
  | {
      name: "banana";
      color: "yellow";
    }
  | {
      name: "orange";
      color: "orange";
    };

type TransformedFruit = {
  [F in Fruit as F["name"]]: `${F["name"]}:${F["color"]}`;
}[Fruit["name"]];
```

