---
title: 03i - Replication
tags:
  - aws
---
## What is it?

S3 has two replication features which allow objects to be replicated between **SOURCE** and **DESTINATION** buckets in the same or different AWS accounts

**Cross-Region Replication (CRR)** is the process used when Source and Destination are in different AWS regions

**Same-Region Replication (SRR)** is used when the buckets are in the same region.

Make sure to checkout: [What is not replicated](https://docs.aws.amazon.com/AmazonS3/latest/dev/replication-what-is-isnot-replicated.html)

There are some slight differences when it comes to differences between *same account* and *different account* replication.

![[Pasted image 20231006141002.png]]

## Replication Options Available

- What to replicate? The default is *all objects*, but this can be a subset
- You can also configure which storage class the replication will use (default is to maintain the existing)
- Can define the *ownership* - default is the source account
- Can do **Replication Time Control** (*RTC*) - This adds a guaranteed 15min replication

## Considerations

- *By default* is is **not retroactive** & version needs to be *on*. This means you cannot do replication without versioning.
	- Batch replication can be used to replicate existing objects, this needs to be configured though
- *One-way replication* source to destination
	- You can configure *bi-directional*
- Replication can handle undecrypted, SSE-S3 & SSE-KMS (*with extra config*) and SSE-C
- Source bucket owner *needs* permissions to objects
- No replication for system events, Glacier, or Glacier Deep Archive
- No deletes are replicated between buckets (but this can be added - *DeleteMarkerReplication*)

## Why use replication?

- **SRR** - Log Aggregation
- **SRR** - Prod and Test Sync
- **SRR** - Resilience with strict sovereignty
- **CRR** - Global resilience improvements
- **CRR** - Latency Reduction

## How to do cross-region replication

1) Head to S3 and create a bucket
2) Edit the bucket and enable [[03b - S3 Static Website Hosting#Creating a Static Site in S3]]l
3) Create a new bucket (good to name it something about it being a *destination bucket*)
	1) Make it in a different region
	2) Make it public
	3) Create bucket
	4) Enable destination bucket as a static website like step 2
4) Go to source bucket
	1) Go to management tab
	2) Create a replication rule
	3) Enable versioning
	4) Create a rule name and keep enabled
	5) You can now choose the scope, in this case we will change it to all objects in the bucket
	6) Select your destination bucket
	7) Enable versioning on your destination bucket
	8) Give replication the correct IAM Role (you may need to create a new role, if you do not have one you need)
	9) Save
	10) Choose if you want to replicate existing
5) Upload your site to *source* and you should see the replication occur to your *destination* (this may take a little bit of time)
6) When deleting, follow normal steps and remember to delete the created role if you chose to do so.


