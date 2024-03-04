---
title: 03n - Object Lock
tags:
  - aws
---
## What is it?

You can use S3 Object Lock to store objects using a _write-once-read-many_ (WORM) model. It can help you prevent objects from being deleted or overwritten for a fixed amount of time or indefinitely. You can use S3 Object Lock to meet regulatory requirements that require WORM storage, or add an extra layer of protection against object changes and deletion.

### Notes

- Object lock can be enabled on *new* buckets (Support request needed for existing)
- It requires *versioning* to be enabled, which means *individual versions* are locked
- It is made up of a [[#Retention Period]] and [[#Legal Hold]]. You can have Both, either or none of these.
- A bucket can have *default* object lock settings

## Retention Period

- You can specify *days & years* for how long it will be applied
- There are 2 modes:
	- **Compliance**: Can't be adjusted, deleted or overwritten
		- This includes the account root user
		- And until the retention expires
	- **Governance**: Special *permissions* can be granted allowing lock setting to be adjusted
		- This can be done using the `s3:BypassGovernanceRetention` permission as well as providing a header with their request `x-amz-bypass-governance-retention:true` (this is console ui default)

## Legal Hold

- Set on an *object version* - ON or OFF
- There is no retention period
- This would mean NO deletes or changes until removed
- This would require an extra permission `s3PutObjectLegalHold` to add or remove
- This is to prevent accidental deletion of critical object versions

![[Pasted image 20231009164804.png]]