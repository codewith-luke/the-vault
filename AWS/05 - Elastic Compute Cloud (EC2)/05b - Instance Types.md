---
title: 05b - Instance Types
tags:
  - aws
---
### Useful Links

- [Instance Types](https://aws.amazon.com/ec2/instance-types/)
- [Instance Type Costs](https://instances.vantage.sh/)

## Choosing an EC2 Type

When choosing an EC2 type you are doing so based on a few different things:

- Raw CPU, Memory, Local Storage Capacity and Type
- Resource Ratios (One instance may have more memory or less storage)
- Storage and Data Network Bandwidth
- System Architecture / Vendor
- Additional features and capabilities (Like GPU's etc.)

### EC2 Groupings

There are 5 main categories for EC2 instances:

- **General Purpose** - Default - Diverse workloads, equal resource ratio
- **Compute Optimized** - Media Processing, HPC, Scientific Modelling, gaming, machine learning
- **Memory Optimized** - Processing large in-memory datasets, some database workloads
- **Accelerated Computing** - Hardware GPU, field programmable gate arrays (FPGAs)
- **Storage Optimized** - Sequential and random IO - scale-out transactional databases, data warehousing, Elasticsearch, analytics workloads

## Decoding EC2 Types (naming of EC2 instance types)

![[Pasted image 20231205092215.png]]

### EC2 Categories

![[Pasted image 20231206085022.png]]
