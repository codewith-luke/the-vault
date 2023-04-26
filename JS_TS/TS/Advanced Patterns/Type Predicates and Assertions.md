https://www.typescriptlang.org/docs/handbook/2/narrowing.html#using-type-predicates

https://www.typescriptlang.org/docs/handbook/release-notes/typescript-3-7.html#assertion-functions

# Combining assertions with Predicate

When running some code, there are times when you do not want to have to modify your logic to check if something is a specific type. You can use a combination of predicates with assertion function in order to achieve this:


```ts
interface User {
  id: string;
  name: string;
}

interface AdminUser extends User {
  role: "admin";
  organisations: string[];
}

interface NormalUser extends User {
  role: "normal";
}

function assertUserIsAdmin(
  user: NormalUser | AdminUser,
): asserts user is AdminUser {
  if (user.role !== "admin") {
    throw new Error("Not an admin user");
  }
}

assertUserIsAdmin(user);
```

So in this example if we pass in a user object that is an admin. What will happen is as long as it resolves as truthy and does not throw we then use `asserts user is AdminUser`  to essentially cast our user as an `AdminUser`.

# Avoid the worst TS error with Assertions

Basically don't do the above example with `const test = () => {}` arrow functions.

# Combining Type Predicates with Generics

When it comes to Type Predicates it is important to remember you can take arguments of functions and use them as well to help with inference:

```ts
interface DOMNodeExtractorConfig<T, Result> {
  /**
   * Here, node is T lets you specify that
   * isNode takes in a type predicate.
   */
  isNode: (node: unknown) => node is T;
  transform: (node: T) => Result;
}

const createDOMNodeExtractor = <T, TResult>(
  config: DOMNodeExtractorConfig<T, TResult>,
) => {
  return (nodes: unknown[]): TResult[] => {
    return nodes.filter(config.isNode).map(config.transform);
  };
};
```

So in the above what we have done is we have a generic `T` and we are wanting to say that the `isNode` function will take an unknown. However when we return that unknown it `is` the type `T` generic. Which is really helpful to infer types.

# Combining [[Branded Types]] and Predicates

```ts
type Valid<T> = Brand<T, "Valid">;

interface PasswordValues {
  password: string;
  confirmPassword: string;
}

const isValidPassword = (
  values: PasswordValues,
): values is Valid<PasswordValues> => {
  if (values.password !== values.confirmPassword) {
    return false;
  }
  return true;
};
```

In the above when used in an if statement (as predicates need to be truthy). That when the values passed into `isValidPassword` will then be cast to a `Valid<PasswordValues>`. It is important to note that we are still returning a boolean. We have just ensured our types are cast correctly based on some conditions within the `isValidPassword`