---
title: 02j - CloudTrail Essentials
tags:
  - aws
---
## What is it?

CloudTrail Is a product which logs API calls and account events.

It's very often used to diagnose security or performance issues, or to provide quality account level traceability.

It is enabled by default in AWS accounts and logs free information with a 90 day retention.

It can be configured to store data indefinitely in S3 or CloudWatch Logs.

In this lesson I detail the theory and architecture of the product.

- Regional service
- Logs API calls/activities as a CloudTrail Event
- Stores last 90 days of events in Event History, enabled by default, no cost for 90 day history
- To customize the service you need to create 1 or more Trails
- It also tracks Management and Data events
- AWS services logged to CloudTrail will log based on the region they are in. If they are a Global service this will be logged to *us-east-1*.
- If you create a Trail you can store this into a S3 Bucket. This is useful to get around the standard 90 day. This will cost based on the storage
- You can also put this data into CloudWatch Logs, which is more powerful than S3
- *NOT* real time. There is about a 15min delay

## How to create a Data Trail

1) Head to CloudTrail
2) Hit the burger menu and click trails
3) Create a new trail
	- Depending on if you want it for all accounts tick the `Enable for all accounts in my organization`
4) Check the CloudWatch toggle if you wish to send it through to there
5) Create trail