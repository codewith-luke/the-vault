## Extract from String with Mapped Types, Template Literals, and infer.

There are a few things going on here for us to understand. Below is the finished code. We will now break it down:

```ts
type UserOrganisationPath = "/users/:id/organisations/:organisationId";

type ExtractPathParams<TPath extends string> = {
  [K in S.Split<TPath, "/">[number] as K extends `:${infer P}`
    ? P
    : never]: string;
};
```

The desired outcome of the above is to have `{id: string, organisationId: string}`. In order to achieve this we need to extract and remap the strings from the original then map and create an object from that.

To start we take the original string, using `ts-tools` we then split the string into a tuple. Then make use `[number]` to iterate and convert that into a union:

```ts
S.Split<TPath, "/">[number] // users | :id | organisaions | :organisationId
```

Now that we have a union we can then build our mapped type:

```ts
type ExtractPathParams<TPath extends string> = {
  [K in S.Split<TPath, "/">[number]]: string;
```

However this will iterate over each key. We only want the keys with `:` so to do that we take `K` and using extends to check it has a `:` we then use `infer` to extract our the part we care about for our new key:

```ts
K extends `:${infer P}`
    ? P
    : never]
```

We can then bring this all together and will result in our desired object.


## Transform an Object/Interface into a Discriminated Union

The solution to this problem looks as follow:

```ts
interface Attributes {
	id: string;
	email: string;
	username: string;
}

type MutuallyExclusive<T> = {
  [K in keyof T]: Record<K, T[K]>;
}[keyof T];

// {id: string} | {email: string} | {username: string}
```

To break it down lets go over each section. First we want to take our interface and go over each key:

```ts
 [K in keyof T]: T[K];
```

Now the above is a simplified version where we would just have an object with our `$key: string`. However in our case we want to create a union of objects that have the correct types. 

So we need to first create a `Record` of with our desired key and its type:

```ts
  [K in keyof T]: Record<K, T[K]>;
```

Now the issue here is that will give us an object of objects:

```ts
{
	id: {
		id: string
	},
	email: {
		email: string
	},
	username: {
		username: string
	}
}
```

To now convert this into a union we can take our type and append `[]` to the keys we want to iterate over using `keyof`:

```ts
type MutuallyExclusive<T> = {
  [K in keyof T]: Record<K, T[K]>;
}[keyof T];
```

What is useful with the above is that using this type you have to parse one of the options to the assignment:

```ts
type ExclusiveAttributes = MutuallyExclusive<Attributes>;

const example: ExclusiveAttributes = {} // Will error as we have to pass at least having one of the defined Attributes
```

## Transform a Discriminated Union with Unique Values to an Object

Taking a discriminated union we want to then transform that into an object that containers never if no `search` property is available:

```ts
type Route =
  | {
      route: "/";
      search: {
        page: string;
        perPage: string;
      };
    }
  | { route: "/about" }
  | { route: "/admin" }
  | { route: "/admin/users" };

type RoutesObject = {
  [R in Route as R["route"]]: R extends { search: infer S } ? S : never;
};

// {
//    "/": {
//       page: string;
//       perPage: string;
//    };
//    "/about": never;
//    "/admin": never;
//    "/admin/users": never;
//  }

```

## Recursive Deep Partial

You can actually recursively call types in Typescript. This makes it useful for iterating over deeply nested objects. Here we want to create an deep partial object. In order to do so we need to first iterate over the top level properties and then work our way down. The end solution looks as follows:

```ts
type DeepPartial<T> = T extends Array<infer U>
  ? Array<DeepPartial<U>>
  : { [K in keyof T]?: DeepPartial<T[K]> };

type MyType = {
  a: string;
  b: number;
  c: {
    d: string;
    e: {
      f: string;
      g: {
        h: string;
        i: string;
      }[];
    };
  };
};

type Result = DeepPartial<MyType>;
```

Walking over deep partial we will start with:

```ts
type DeepPartial<T> = { [K in keyof T]?: DeepPartial<T[K]> };
```

Here this may seem like enough. Each of our properties are technically optional. We iterate over each key and then carry on down. 

The issue with this is when we hit our array prop `g`. Although technically optional, it still allows us to pass undefined. So we have to first check if it is an array, extract the properties in the array and then recursively run deep partial on all of it's properties:

```ts
T extends Array<infer U>
  ? Array<DeepPartial<U>>
  : { [K in keyof T]?: DeepPartial<T[K]> };
```
