# Classes and [[Type Predicates and Assertions]]

In order to make use of properties on a class and use those with Type Predicates you have to use the following syntax:

```ts
class Form<TValues> {
  error?: string;

  constructor(
    public values: TValues,
    private validate: (values: TValues) => string | void,
  ) {}

  isInvalid(): this is Form<TValues> & { error: string } {
    const result = this.validate(this.values);

    if (typeof result === "string") {
      this.error = result;
      return true;
    }

    this.error = undefined;
    return false;
  }
}
```

So here we have said `this is Form<TValues>`  to first explain that it is to be cast as itself. But we then extend using `&` to then say that `error: string`. Also instead of `this is Form<TValues>` you can also do `this is this`.

The above applies to Assertions as well.

# Typesafe Builder Pattern

Below is an example of a typesafe builder pattern. The important part to take now of here is the return of the generic `BuilderTuple<TList extends any[] = []>`. Passing in a default of `[]` we have said that this is our starting point. Then we look to the return of `push` and `unshift`. Here we have said take the previous types and merge them. This means that whenever we chain push and unshift we will have typesafe values.

```ts
export class BuilderTuple<TList extends any[] = []> {
  list: TList;

  constructor() {
    this.list = [] as any;
  }

  push<TNum extends number>(num: TNum): BuilderTuple<[...TList, TNum]> {
    this.list.push(num);

    return this as any;
  }

  unshift<TNum extends number>(num: TNum): BuilderTuple<[TNum, ...TList]> {
    this.list.unshift(num);

    return this as any;
  }
}

const builderBeforePush = new BuilderTuple();
const listBeforePush = builderBeforePush.list;

const builderAfterPush = builderBeforePush.unshift(3).unshift(2).unshift(1);
const listAfterPush = builderAfterPush.list;
```

Likewise the above can be achieved with things like Maps with the & operator to merge:

```ts
 set<K extends string>(key: K, value: string): TypeSafeStringMap<Record<K, string> & TMap> {
    (this.map[key] as any) = value;

    return this;
  }
```

# Dynamic Middleware

Below is an example of a dynamic middleware that basically extends each time we call the `use` function. Lets go over:

1) First have `class DynamicMiddleware<TInput, TOutput>`. This is essentially our starting point. Where we then pass in our first middleware and push that into the array via the constructor.
2) The use is where the magic happens. First we define a generic `<NewTOutput>` that we use to infer the output of the middleware we pass in. 
3) We then use that generic to create a new middleware `Middleware<TOutput, NewTOutput>` and then say that this `use` will then return our DynamicMiddleware that is now extended with the `NewTOutput`. 
This has to be cast as `any` as we have to trick TS into defining our class with the correct type which we then tell it what it will be thereafter.

```ts
class DynamicMiddleware<TInput, TOutput> {
  private middleware: Middleware<any, any>[] = [];

  constructor(firstMiddleware: Middleware<TInput, TOutput>) {
    this.middleware.push(firstMiddleware);
  }

  use<NewTOutput>(
    middleware: Middleware<TOutput, NewTOutput>
  ): DynamicMiddleware<TInput, NewTOutput> {
    this.middleware.push(middleware);

    return this as any;
  }

  async run(input: TInput): Promise<TOutput> {
    let result: TOutput = input as any;

    for (const middleware of this.middleware) {
      result = await middleware(result);
    }

    return result;
  }
}

const middleware = new DynamicMiddleware((req: Request) => {
  return {
    ...req,
    // Transforms /user/123 to 123
    userId: req.url.split("/")[2],
  };
})
  .use((req) => {
    if (req.userId === "123") {
      throw new Error();
    }
    return req;
  })
  .use(async (req) => {
    return {
      ...req,
      user: await fetchUser(req.userId),
    };
  });
```