---
title: 03a - S3 Resource Policies
tags:
  - aws
---
## How to secure Buckets

The base line of S3 is that it is *private* by *default*. The only identity that has initial access is the account root user of the account which own that bucket, the account that created it. Otherwise has to be explicitly granted. 

This can be done in the form of bucket policies, these are a type of [[@Terms#Resource Policy]].

## Block Public Access

Public access is read access to anything in your bucket. Block public access added a further boundary for security.

The idea behind this is that it just applies to public access, no matter what the bucket policies say. They only apply to anonymous [[@Terms#Principal]]. It is a full override, or fail safe.

![[Pasted image 20230914090808.png]]



*NOTE:* There is also the legacy [ACL](https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html) way of managing permissions. This is not generally recommended but good to know it exists, it is way less flexible and recommended. 



