---
title: 07f - Enhanced Networking & EBS Optimized
tags:
  - aws
---
### What is enhanced networking?

Enhanced networking is the AWS implementation of SR-IOV, a standard allowing a physical host network card to present many logical devices which can be directly utilized by instances.

This means lower host CPU usage, better throughput, lower and consistent latency

- No charge - available on most EC2 Types
- Higher I/O & Lower host CPU usage
- Higher packets-per-second (**PPS**)
- Consistent lower latency

![[Pasted image 20240229084748.png]]

### What is EBS Optimized?

EBS optimisation on instances means dedicated bandwidth for storage networking - separate from data networking.

- EBS = Block storage overt the network
- Historically network was shared (data & EBS)
- It basically means *dedicated capacity* has been provided for EBS usage
- Most instances support and have enabled by default
	- If it doesn't will have some support but enabling costs extra
