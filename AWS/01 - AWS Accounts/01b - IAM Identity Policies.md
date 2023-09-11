---
title: IAM Identity Policies
tags:
  - aws
---
## What are they?

Identity Policies are attached to AWS identities and either ALLOW or DENY access to AWS resources.

![[Pasted image 20230904105654.png]]

Policies are made up of one or more statements. A statement can be broken up into the following:

- **Sid** - Optional statement field that declares what it does. This is for the reader to understand what the statement does.
- **Effect** - This is either *allow* or *deny*. This is just to tell what the statement will do.
- **Action** - Can list a specific action. The format is *{service}:{operation}*. Or as per example above you have a wild card which could be any. Alternatively you can give a list of independent actions.
- **Resource** - This matches AWS resources.

In the above you may notice these statements overlap. The first statement basically says that any action can be performed on any S3 bucket, full access. However the 2nd statement takes priority due to:

- If there is an explicit *deny* then that will be what is used. Nothing can overrule that.
- The next priority is explicit *allows*, these will take effect *unless* there is an explicit *deny*.
- If there is no explicit then the *default* *deny* will take effect. With the exception of the account root user, all other identities start off with no access to AWS resources.

![[Pasted image 20230904110816.png]]

## Types of Policies

- **Inline** - This is where apply the policies to each account that needs it. This comes with the issue that if you need to update a policy, everywhere that uses that policy needs to be updated. You would generally use these for special/exceptional allow/denies.
- **Managed Policy** - These are created as their own object, then you can apply this to each account. So one source of truth. This should be used for common access writes for your organisation.

