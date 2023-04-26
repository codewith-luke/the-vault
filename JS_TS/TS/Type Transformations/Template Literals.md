## String Patterns

With the below code what we are doing here is saying I want a string that starts with a `/` and the type being passed must be a string:

```ts
type Route = `/${string}` 

const goToRoute = (route: Route) => {}

goToRoute("/users/1")

// ts-expect-error
goToRoute("users/1")
```

We can then start to combine pattern matching with utility functions like Extract:

```ts
type Routes = '/users' | '/users/:id' | '/posts' | '/posts/:id';

type DynamicRoutes = Extract<Routes, `${string}:${string}`>;
// '/users/:id' | '/posts/:id'
```

This says match anything with a string before the `:` and any string after it as well.

## Combining Inference with String Literals and Records

In the below example we are creating a new object with inference and string literals.

First taking an object and extracting the types out of it and then appending `_alt_payment_method` onto it, this creates a union of these new strings.

```ts
const TypePurchases = {
	firstSelfHostLicensePurchase: 'first_purchase',
	renewalSelfHost: 'renewal_self',
	monthlySubscription: 'monthly_subscription',
	annualSubscription: 'annual_subscription',
} as const;

type MetadataGatherWireTransferKeys = `${ValueOf<typeof TypePurchases>}_alt_payment_method`
```

This generates the below:
```ts
// Generated union
type MetadataGatherWireTransferKeys =
  | "first_purchase_alt_payment_method"
  | "refewal_self_alt_payment_method"
  | "monthly_subscription_alt_payment_method"
  | "annual_subscription_alt_payment_method"
```

We can then create a new record with specified types from our newly created union:
```ts
type CustomerMetadataGatherWireTransfer = Partial<
  Record<MetadataGatherWireTransferKeys, string>
>
```

This will create the following:
```ts
type CustomerMetadataGatherWireTransfer = {
  first_purchase_alt_payment_method?: string | undefined
  refewal_self_alt_payment_method?: string | undefined
  monthly_subscription_alt_payment_method?: string | undefined
  annual_subscription_alt_payment_method?: string | undefined
}
```

