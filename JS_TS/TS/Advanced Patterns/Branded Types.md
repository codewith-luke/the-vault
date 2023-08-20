# Creating Reusable Validity Checks with Branded Types and Type Helpers

The following example checks if a password is valid. We only want to be able to pass our password around as long as it is valid. In order to do so we can use branded types to create a `Valid` branded type:

```ts
type Brand<T, TBrand> = T & { [brand]: TBrand };

type Valid<T> = Brand<T, "Valid">;

interface PasswordValues {
  password: string;
  confirmPassword: string;
}

const validatePassword = (values: PasswordValues): Valid<PasswordValues> => {
  if (values.password !== values.confirmPassword) {
    throw new Error("Passwords do not match");
  }

  return values as Valid<PasswordValues>;
};

const createUserOnApi = (values: Valid<PasswordValues>) => {
  // Imagine this function creates the user on the API
};

```

Here we only want `createUserOnApi` to accept valid passwords. However we need to ensure that our `validatePassword` first checks and then if is valid returns our new branded type. This accepts a type and marks it as "Valid".

# Using Index Signatures and Branded Types

The example below takes branded types and essentially creates 2 options and what type you would get back using index signatures.

```ts
type PostId = Brand<string, "PostId">;
type UserId = Brand<string, "UserId">;

interface User {
  id: UserId;
  name: string;
}

interface Post {
  id: PostId;
  title: string;
}

const db: {
  [id: PostId]: Post;
  [id: UserId]: User;
} = {};
```