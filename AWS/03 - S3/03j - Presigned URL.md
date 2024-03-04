---
title: 03j - Presigned URL
tags:
  - aws
---
## What is it?

Presigned URL's are a feature of S3 which allows the system to generate a URL with access permissions encoded into it, for a specific bucket and object, valid for a certain time period.

Currently if you wanted to give someone access to a bucket you would need to do one of the following:

- Give an AWS identity
- Provide AWS credentials
- Make public

None of these are ideal for short term access to a bucket. This can also be viewed as a security risk.
The solution to this is to use *presigned urls*.

![[Pasted image 20231009145533.png]]

### Useful Points

- You can create a URL for an object you have *no access to*
	- You still won't have access, but it is possible
- When using the URL, the permissions match the identity that *generated it*.
	- Access denied could mean the generating ID never had access or no longer does
- **Don't** generate with a role. URL stops working when temporary credentials expire. Always use long term identities (IAM User).

## How to

1) Create a basic S3 Bucket
2) Upload something to your bucket like an image
3) Open the object in your bucket
4) Open the cloud shell in the top bar (CLI in AWS browser)
5) `aws s3 ls` will show you your buckets
6) `aws s3 presigned ${uri} --expires-in 180` 
	- This will generate your presigned URL that you should be able to now view the asset you put in the URI for that allocated time.
	- This will be just a basic GET request
7) Move to IAM and add a new policy to your admin user
```JSON
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "VisualEditor0",
      "Effect": "Deny",
      "Action": "s3:*",
      "Resource": "*"
    }
  ]
}
```
- The important thing to note here is that because the user that generated the token was the admin user that presigned URL would be denied. As per our policy rules.
- Remember to remove this policy after you are done trying this
