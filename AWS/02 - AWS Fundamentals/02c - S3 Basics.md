---
title: 02c - S3 Basics
tags:
  - aws
---

This can be considered as your default storage when it comes to AWS.

- *Global* storage platform - *regional* based/resilient 
- Public service, unlimited data & multi-user
- Moves, audio, photos, large data sets...
- Economical & accessed via UI/CLI/API/HTTP
- Made up of Objects & Buckets
	- *Objects* are things like your movies or data sets
	- *Buckets* are containers for objects

## Objects

Objects have a key value, if you know the key value and the bucket you are able to retrieve the object.

An object also has a value which is data stored in binary. This can range from a size of *0 Bytes - 5TB*

Objects also contain:
- Version ID
- Metadata
- Access Control
- Sub-resources

## Buckets

Are created in a specific AWS region. It never leaves that region unless configured.

Bucket names need to be **Globally Unique**, this means no one can have the name other than you.

Buckets can hold an unlimited number number of objects, this makes it an infinitely scalable storage system.

*NOTE*: It is also important to note that S3 is a simple storage system. Everything is flat, meaning it is all stored at the root level.

When it comes to `folders` in S3 there is none. If you see something like `old/my-image` this may appear as a folder in S3. It is not. It is considered a *prefix*.

## Summary

- Globally unique
- 3-63 characters, all lowercase no underscores
- Start with a lowercase letter or a number
- Can't be IP formatted e.g. 1.1.1.1
- Buckets - 100 soft limit, 1000 hard per account
- Unlimited objects, each object being 0 Bytes to 5TB
- Objects look like Key = Name, Value = Data
- Buckets by default are private when created

## S3 Patterns & Anti Patterns

- S3 is an object store - not a file or a block
- You **can't mount** an S3 bucket
- Great for large scale data storage, distribution or upload
- Great for *offload* of data. Think of shrinking your instance size off to S3
- Allows for *input* and/or *output* to *many* AWS products

### Creating a S3 Bucket

1) Navigate to S3 Service in dashboard, then click create bucket
2) Select relevant settings
3) Create the bucket

