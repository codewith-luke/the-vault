---
title: 03l - S3 Events
tags:
  - aws
---
## What is it?

The Amazon S3 notification feature enables you to receive notifications when certain events happen in your bucket. To enable notifications, you must first add a notification configuration that identifies the events you want Amazon S3 to publish and the destinations where you want Amazon S3 to send the notifications. You store this configuration in the _notification_ subresource that is associated with a bucket

- Notification generated when events occur in a bucket
	- Can be delivered to *SNS, SQS and Lambda functions*
- Object **Created** (Put, Post, Copy, CompleMultiPartUpload)
- Object **Delete** (Delete, DeleteMarkerCreated)
- Object **Restore** (Post (Initiated), Completed)
- **Replication** (OperationMissedThreshold, OperationReplicatedAfterThreshold, OperationNotTracked, OperationFailedReplication)

![[Pasted image 20231009162924.png]]