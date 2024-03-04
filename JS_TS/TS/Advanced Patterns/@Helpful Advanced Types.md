https://basarat.gitbook.io/typescript/
https://codemix.com/

# Make Safe Result

```ts
/**
 * First, create a type helper that represents
 * the Result that we'll get from our safe function
 */
type Result<T> =
  | {
      ok: true;
      value: T;
    }
  | {
      ok: false;
      error: unknown;
    };

/**
 * Next, make a function that wraps the function
 * you pass it with a try/catch, then executes it
 */
export const makeSafe =
  <TArgs extends any[], TReturn>(
    func: (...args: TArgs) => TReturn
  ) =>
  (...args: TArgs): Result<TReturn> => {
    try {
      return {
        value: func(...args),
        ok: true,
      };
    } catch (e) {
      return {
        error: e,
        ok: false,
      };
    }
  };


/**
 * Wrap any function you want to error check with this
 * makeSafe wrapper
 */
const randomlyFail = makeSafe((input: number) => {
  if (input > 0.5) {
    throw new Error("oops");
  }
  return {
    input,
  };
});

```

# Create a Type-Safe request Handler with Zod and Express

```ts
// 1) First we ensure that we have the correct generics
// The body should extend record otherwise default to any
const makeTypeSafeHandler = <
  TQuery extends ParsedQs = any,
  TBody extends Record<string, any> = any
>(
  config: {
	// 2) We pass in our generics to zod schemas so 
	// inference works as expected
    query?: z.Schema<TQuery>;
    body?: z.Schema<TBody>;
  },
  // 3) We setup our request handlers to give them
  // the expected generics,these have to match to
  // ensure we pass the correct types and infer correctly
  handler: RequestHandler<any, any, TBody, TQuery>
): RequestHandler<any, any, TBody, TQuery> => {
  return (req, res, next) => {
    const { query, body } = req;
    if (config.query) {
      try {
        config.query.parse(query);
      } catch (e) {
        return res.status(400).send((e as ZodError).message);
      }
    }
    if (config.body) {
      try {
        config.body.parse(body);
      } catch (e) {
        return res.status(400).send((e as ZodError).message);
      }
    }
    return handler(req, res, next);
  };
};
```

# Building a Dynamic Reducer (Builder)

```ts
type PayloadsToDiscriminatedUnion<T extends Record<string, any>> = {
  [K in keyof T]: { type: K } & T[K];
}[keyof T];

// 1) First we make generics for State and Payload
// we also ensure our payload map is constrained as per our 
// PayloadsToDiscriminatedUnion abov: Record<string, any>
// important to also have a default set to {}
export class DynamicReducer<
  TState,
  TPayloadMap extends Record<string, any> = {}
> {
  // 2) here we dfine our handlers as a 
  // record made up of our state and any payload that returns our state
  // we are using any as it is constrained to our DynamicReducer
  // and gets inferred later
  private handlers = {} as Record<
    string,
    (state: TState, payload: any) => TState
  >;
  // 3) We create generics for our type and payload which extends
  // and object
  addHandler<TType extends string, TPayload extends object>(
    type: TType,
    // 4) We ensure our handler here uses that generic TPayload
    // as per (2) the any would no longer matter here and it would
    // be as TPayload
    handler: (state: TState, payload: TPayload) => TState
    // 5) We return our class with hour state and payload map
  ): DynamicReducer<TState, TPayloadMap & Record<TType, TPayload>> {
    this.handlers[type] = handler;

    return this;
  }
  // 6) We ensure we pass the state and also use the PayloadsToDiscriminatedUnion
  // and pass it our PayloadMap from (1)
  reduce(
    state: TState,
    action: PayloadsToDiscriminatedUnion<TPayloadMap>
  ): TState {
    const handler = this.handlers[action.type];
    if (!handler) {
      return state;
    }

    return handler(state, action);
  }
}

interface State {
  username: string;
  password: string;
}

const reducer = new DynamicReducer<State>()
  .addHandler(
    "LOG_IN",
    (state, action: { username: string; password: string }) => {
      return {
        username: action.username,
        password: action.password,
      };
    }
  )
  .addHandler("LOG_OUT", () => {
    return {
      username: "",
      password: "",
    };
  })
  .addHandler("UPDATE_USERNAME", (state, action: { username: string }) => {
    return {
      ...state,
      username: action.username,
    };
  });
```

# Add a custom element to JSX

```ts
declare global {
  namespace JSX {
    interface IntrinsicElements {
      "custom-solution-element": {
        children?: React.ReactNode;
      };
    }
  }
}
```

# Debug Prettify Helper

```ts
type Prettify<T> = {
	[K in keyof T]: T[K]
} & {};
```