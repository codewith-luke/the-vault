---
title: 03c - Object Versioning and MFA Delete
tags:
  - aws
---
## What is versioning?

Without versioning on a bucket. The object is identified using it's **name**. Versioning lets you store multiple versions of an object.
## Bucket Versioning States?

By default versioning is disabled. However it is important to know that if you do enable it, it cannot be disabled. You can also suspend a bucket and this can then be re-enabled. This is important to know because if you have versioning it will take up space for each version, as a result could be more space being used.

An object contains a `KEY` and a `id`. When versioning is disabled this `id` is set to `null`. When versioning is enabled this `id` will then be set.

![[Pasted image 20230926084512.png]]

### Deleting

When deleting an object what S3 will do is inset something called a delete marker. This will not actually delete the objects, but will make it appear as if it has. You can then also delete the delete marker and this will restore the previous versions.

![[Pasted image 20230926085513.png]]

You can also delete a the current version. If you do that it will then fall-back to the previous version.

## MFA Delete

This is enabled in *versioning configuration*.
This as the name suggests, will require MFA is required to change bucket versioning state and to delete versions.

- You need to provide the `MFA` + Code Passed with API Calls
## How to

**Uploading**
1) Head over to S3 and create a new bucket with your desired settings
	- Make sure to enable versioning under the heading versioning
2) Upload any files you wish to have
3) You can head to objects tab and click the toggle to *show versions*
4) Upload a object that you already have with the same name
	- Make sure show versions is enabled and you should see 2 different versions of the same object

**Creating Delete Marker**
1) Turn **OFF** *show versions* select your object and delete
2) This will create a delete marker if you enable *show versions*
3) You can do select the delete marker if you wish to restore the previous versions

**Deleting a Version**
1) Turn **ON** *show versions* select object and delete
2) This will delete a single version and cannot be restored