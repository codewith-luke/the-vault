---
title: 01c - IAM Users
tags:
  - aws
---
## What are they?

IAM Users are an identity used for anything requiring long-term AWS access e.g. Humans, Applications, service accounts.

### Principal

Represents an entity trying to access and AWS account, at this point it is unidentified. It needs to authenticate and be authorized to do anything.

Authentication happens where [[@Terms#Principal]] proves to IAM that it is an identity that it claims to be.

This is done via:
- Username + Password
- Access Keys

Once authenticated it is then known as a *authenticated identity*. 

### Amazon Resource Names (ARN)

Uniquely identify resources within any AWS accounts. This can be used to identify a single resource or groups (through wildcards).

They look something like:

![[Pasted image 20230905091029.png]]

The difference between these two is:

1) References an actual *bucket* in S3.
2) References anything in the *bucket*, **not** the bucket itself.

These two ARN's do not overlap. They reference specific aspects.

![[Pasted image 20230905091049.png]]

## Useful Things

- Max **5000** IAM Users per account
- IAM user can be a member of **10** groups
- This creates system design impacts
- If you encounter a situation that you need large scale of users. This generally means you should be looking into **IAM Roles & Identity Federation**