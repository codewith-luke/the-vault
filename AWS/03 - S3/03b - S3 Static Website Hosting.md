---
title: 03b - S3 Static Website Hosting
tags:
  - aws
---
## Good for?

- Offloading
- Out-of-band pages
- Simple static sites

## Creating a Static Site in S3

1) Head to S3 and *create bucket*
2) Enter Bucket Name (make sure if you have a domain you want to use that you must use a DNS  formatted name)
	- i.e. *top10.animals4life.io*
3) Uncheck block all public access
	- This gives you permission to grant public access. It does not give public access.
4) Create bucket
5) Go to your bucket, select properties tab and got to the bottom to *Static Website Hosting* then edit and enable.
6) Select *Host a static website*
	- Provide index and error documents
7) Save and then copy the URL under static website hosting
8) Go to objects and click on upload
	- Upload any files and folders that you need for your site
9) Go to permissions tab
	- Edit bucket policy and use the following policy.
	- Make sure to change the *examplebucket* to your S3 bucket for your static site
```json
{
    "Version":"2012-10-17",
    "Statement":[
      {
        "Sid":"PublicRead",
        "Effect":"Allow",
        "Principal": "*",
        "Action":["s3:GetObject"],
        "Resource":["arn:aws:s3:::examplebucket/*"]
      }
    ]
  }
```
10) You can then use Route53 if you configured a custom domain for step 2.
