---
title: 03f - Server Side Encryption SSE
tags:
  - aws
---
## Client vs Server Side Encryption

- Client side means that the users/app side it has been encrypted, which means through the whole process it is encrypted.
- Server side means that in transit it is in it's original form. Once it hits the server it is then encrypted.

### Encryption Options

1) **Client-Side Encryption**

2) **SSE-C** - Server Side Encryption with Customer Provided Keys 

![[Pasted image 20231005125914.png]]

4) **SSE-S3** - Server Side Encryption with AWS S3 Managed Keys (*default*)

- Good default type of encryption. However less control.
- Not good for strong regulated environments and control over keys
- Not good for Rotation of keys
- Not good for Role separation (Can't stop a S3 full admin)
- Encryption shows as AES256

![[Pasted image 20231005130619.png]]

4) **SSE-KMS** - Server Side Encryption with KM Keys stored in AWS KMS

![[Pasted image 20231005131318.png]]

## Summary

![[Pasted image 20231005131403.png]]
## S3 Bucket Keys

- [Source]([https://docs.aws.amazon.com/AmazonS3/latest/userguide/bucket-key.html](https://docs.aws.amazon.com/AmazonS3/latest/userguide/bucket-key.html))

The general idea is that when uploading to S3 and using KMS encryption you have the potential to be throttled. Calls to KMS have a cost and are limited. 

![[Pasted image 20231005140149.png]]

To get around this you make use of **S3 Bucket Keys**. These essentially are a time limited key that would be used to generate DEK's within S3. This offloads the responsibility to S3 and reduces calls to KMS.

![[Pasted image 20231005140345.png]]

### Things to note

- CloudTrail KMS events now show the bucket and so will see less KMS events as well
- Works with *replication*, the object encryption is maintained
- If replicating a plaintext to a bucket using bucket keys the object is encrypted at the destination side
## How to

1) Create an S3 bucket
2) Create a KMS Key
3) Upload some files to your bucket
	- Under properties make sure you head to sever side encryption and specify and encryption key
	- Here you can see S3 and KMS key types
4) Upload