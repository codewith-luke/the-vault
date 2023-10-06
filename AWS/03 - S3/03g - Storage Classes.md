---
title: 03g - Storage Classes
tags:
  - aws
---
## S3 Standard

This is the default. 

- Replicated over at least 3 availability zones
- Provides 11 9's of durability
- When S3 API responds with *HTTP/1.1 200 OK* you know it has been stored
- Billed *GB/m* and per *GB* transfer and then price per *1000 requests*
- Most balanced class of storage
- Makes data available immediate
- Use standard for *frequently accessed data* which is important and not replaceable

![[Pasted image 20231005143324.png]]

## Standard-IA (Infrequent Access)

- Same replication, durability and 1st byte latency is all the same as standard and cost model is also the same. 
- It is a lot cheaper than standard
- But in exchange for being cheaper
	- Retrieval fee
	- Frequent access = increased costs
	- Minimum duration charge of 30 days
	- Min capacity charge of 128KB per object
- Should be *used for long lived data* but *where access is infrequent*
- Don't use for lot's of small files, temporary or frequently accessed or for data which is *not* important or easily replaced

![[Pasted image 20231005143823.png]]
## One Zone-IA

- Cheaper than other classes but comes with a significant compromise
- Still has retrieval fee and min duration fee and capacity charge.
- The main difference is that data stored is only stored in one AZ within a region
- You do get same level of durability
- Used for long lived data, infrequently accessed and for non-critical and easily replaced data

![[Pasted image 20231005144027.png]]

## S3 Glacier - Instant

Like *Standard-IA*. Cheaper storage, more expensive retrieval, longer minimum (*90 days*). It is designed for data you need instantly but not often. 

![[Pasted image 20231005144849.png]]

## S3 Glacier - Flexible

Same availability zone as *S3 Standard*. Has a storage cost which is about 1/6th of Standard. So it is really cost effective. However you should view these items as cold objects.

Tradeoffs:
-  Not immediately available
- Cannot be made publicly accessible and requires a retrieval process which costs more based on how fast:
	- Expedited (1-5min)
	- Standard (3-5h)
	- Bulk (5-12h)
- 40KB minimum billable size

This makes it a good archive option. But it is not the most cheap type of storage.

![[Pasted image 20231005145235.png]]

## S3 Glacier Deep Archive

This can be viewed as data in a frozen state. Same as **Glacier Flexible** but it takes longer:
- Standard (12h)
- Bulk (Up to 48h)

Tradeoffs:
- 40KB min billable size
- 140 day min billable duration

Should be used for archive data that should be barely accessed if ever. Good for data for regulatory archives.

![[Pasted image 20231005145631.png]]
## S3 Intelligent Tiering

Different to all other storages. It contains *5* other storage tiers.

1) Frequent Access
2) Infrequent Access
3) Archive Instant Access
4) Archive Access
5) Deep Archive

The pricing for the above are similar to their relevant counterparts.

![[Pasted image 20231005150415.png]]