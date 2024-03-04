---
title: 03h - Lifecycle Configuration
tags:
  - aws
---
## What is it?

- A set of rules that you apply to a bucket
- Rules consist of actions and can apply to a whole *bucket* or *group of objects*
	- Basically do x if y is true
- There are 2 types of actions
	- *Transition* Actions
		- Change the storage class of the objects affected (e.g. Standard => Standard-IA)
	- *Expiration* Actions
		- Can delete objects or versions based on time periods.
- These configurations offer us a way to manage and automate these processes

You can think of S3 Lifecycle Transitions like a waterfall. Generally though you won't go directly, and go in stages, but you can do direct. It can only go down, not up when using these lifecycle transitions.

*Remember* for ***S3 Standard*** and transitioning to others:
- Smaller objects can cost more (due to minimum size)
- Minimum of 30 days before transition
- A single rule cannot transition or Standard-IA or One Zone-IA and then tor glacier classes within 30 days

![[Pasted image 20231005151744.png]]