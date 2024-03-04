---
title: 05a - Architecture and Resilience
tags:
  - aws
---
## What is it?

EC2 Instances are **virtual machines (OS + Resources)** and run on **EC2 Hosts**. These hosts are shared or dedicated. So either your share with other customers or have your own. However with shared it is important to know you do not have interaction with any other customers.

EC2 is AZ Resilient. So that means if an AZ fails you have to assume that some if not all of your instances in that AZ would as well.

EC2 is AZ locked. So if you are creating your EC2 instances in let's say *AZ-A*. If that AZ fails then everything related to your EC2 could be impacted. This includes things such as subnets, volume, EBS etc. It also means that you cannot connect/share from another AZ.

![[Pasted image 20231205085814.png]]

## What is EC2 good for?

- Traditional **OS + Application** compute
- Long running compute
- Server style applications
- Burst or steady-state load
- Monolithic application stacks
- Migrated application workloads or disaster recovery