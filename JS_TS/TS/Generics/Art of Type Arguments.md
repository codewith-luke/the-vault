# Generics at Different Levels

Sometimes you may only be concerned with the types at a certain level within an object. To achieve this will depend on how you structure your objects and return types but a good way of doing it is to make your generic represent a low level:

```ts
export const getHomePageFeatureFlags = <HomePageFlags>(
  config: {
    rawConfig: {
      featureFlags: {
        homePage: HomePageFlags;
      };
    };
  },
  override: (flags: HomePageFlags) => HomePageFlags
) => {
  return override(config.rawConfig.featureFlags.homePage);
};
```

So in the above we are saying that our `getHomePageFeatureFlags` function will expect a generic. This should represent a specific structure when these arguments are passed in.

```ts
  const EXAMPLE_CONFIG = {
    apiEndpoint: "https://api.example.com",
    apiVersion: "v1",
    apiKey: "1234567890",
    rawConfig: {
      featureFlags: {
        homePage: {
          showBanner: true,
          showLogOut: false,
        },
        loginPage: {
          showCaptcha: true,
          showConfirmPassword: false,
        },
      },
    },
  };
  
 const flags = getHomePageFeatureFlags(
      EXAMPLE_CONFIG,
      (defaultFlags) => defaultFlags
    );
```

# Typed Object Keys

You may want to extract the keys of a passed in object and return those as an array: 

```ts
const typedObjectKeys = <TObject extends object>(obj: TObject) => {
  return Object.keys(obj) as Array<keyof TObject>;
};
```

Here we are checking that our generic is of a type object that we then are able to extract the keys from and in cast it using `as` to then get back the type.

# Make a Generic Wrapper for a Functions

This is useful for creating and inferring your types for wrapper functions. This makes use of utility functions `ReturnType` and  `Parameters`:

```ts
const makeSafe =
  <TFunc extends (...args: any[]) => any>(func: TFunc) =>
  (
    ...args: Parameters<TFunc>
  ):
    | {
        type: "success";
        result: ReturnType<TFunc>;
      }
    | {
        type: "failure";
        error: Error;
      } => {
    try {
      const result = func(...args);

      return {
        type: "success",
        result,
      };
    } catch (e) {
      return {
        type: "failure",
        error: e as Error,
      };
    }
  };
```

Alternatively if this gets too out of control with different utilites you can use:

```ts
const makeSafe =
  <TParams extends any[], TReturn>(func: (...args: TParams) => TReturn) =>
  (
    ...args: TParams
  ):
    | {
        type: "success";
        result: TReturn;
      }
    | {
        type: "failure";
        error: Error;
      } => {
    try {
      const result = func(...args);

      return {
        type: "success",
        result,
      };
    } catch (e) {
      return {
        type: "failure",
        error: e as Error,
      };
    }
  };
```

# Infer the Type of an Array Member

The problem at hand is that we have the following:

```ts
const makeStatus = <TStatuses extends string[]>(statuses: TStatuses) => {
  return statuses;
};
```

This will return an array of strings. However what we really want from this is each member within the statuses array to be our type that we return. To do so we just have to make some small adjustments:

```ts
const makeStatus = <TStatuses extends string>(statuses: TStatuses[]) => {
  return statuses;
};
```

So here what we are saying is that each status must be a string, then inferring each of them in the arguments as an array of the. Which results in:

```ts
const statuses = makeStatus(["INFO", "DEBUG", "ERROR", "WARNING"]);
//  Array<"INFO" | "DEBUG" | "ERROR" | "WARNING">
```



