---
title: 03o - Access Points
tags:
  - aws
---
## What is it?

- [Creating Access Points](https://docs.aws.amazon.com/AmazonS3/latest/dev/creating-access-points.html#access-points-policies)

Amazon S3 Access Points, a feature of S3, simplifies managing data access at scale for applications using shared data sets on S3. Access points are unique hostnames that customers create to enforce distinct permissions and network controls for any request made through the access point.

- They simplify managing access to S3 Buckets
	- Rather than a single bucket with a bucket policy you can create many access points, each with different policies and different network access controls
	- Each access point has its own endpoint address
- Access points can be create via console or CLI with 
	- `aws s3control create-access-point --name {name} --acount-id {id} --bucket {bucket}`

![[Pasted image 20231009165413.png]]