---
title: 06c - Elastic Container Register
tags:
  - aws
---
## What is it?

- Managed *container image registry* service
	- Like docker hub but for AWS
- Each AWS account has a public and private registry
- Each registry can have many repositories
	- And in each repository and contain many images
	- Images can have several tags
- *Public* = R/W requires permissions
- *Private*  = permissions required for all operations (R/W & R/O)
- It is integrated with IAM - Permissions
- Comes built in with an image scanning (this checks things like issues OS and outdated images)
- Has near real time metrics which is integrated into Cloudwatch
- All API actions are put into Cloud Trail
- All events published to Eventbridge
- Has replication for cross-region and cross-account
