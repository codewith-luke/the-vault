---
title: 07d - Placement Groups
tags:
  - aws
---
## What is it?

These are used when you want to achieve the highest performance possible with EC2.
#### Some Terms

- **Cluster** - Pack instance close together
- **Spread** - Keep instances separated
- **Partition** - group of instances spread apart

### Cluster Group

![[Pasted image 20240227085106.png]]

#### Limitations and notes

- Can't span AZs (one only) locked when launching first instance
- Can span VPC peers, but impact performance
- Requires a supported instance type
- Use the same type of instance (not mandatory)
- Launch at the same time (not mandatory, but very recommended)
- Offer 10gbps single stream performance
- Use cases: *Performance, fast speeds, low latency*

### Spread Placement Group

Are instances which are located on separate isolated infrastructure racks in each availability zone. So each instance has it's own networking, power supply separate from any of the other instances

![[Pasted image 20240227085415.png]]

#### Limitations and notes

- Only 7 instances per AZ
- Provide infrastructure isolation
- Each instance runs from a different rack
- Each rack has its own *network* and *power* source
- Not supported for dedicated host instances or hosts
- Use cases: Small number of critical instance that need to be kept separate from each other

### Partition Placement Groups

Why use this over spread? These are designed where infrastructure where you have more than 7 instances per AZ but still need them separate. 

![[Pasted image 20240227090212.png]]
#### Limitations and notes

- 7 Partitions per PZ
- Instances can be placed in a specific partition
	- Or auto placed
- Great for topology aware applications
- HDFS, HBase, and Cassandra
- Contain the impact of failure to part of an pplication