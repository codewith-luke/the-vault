---
title: 05d - Network Interfaces, Instance IP's and DNS
tags:
  - aws
---
## Network Interfaces

Each EC2 Instance will have a primary **ENI (Elastic Network Interface)**. You are able to attach other secondary ENI's but all ENI's must be in the same **AZ**.

Each interface has:

- MAC Address 
- Primary IPv4 Private IP
- 0 or More Secondary IPs
- 0 or 1 public IPv4 Address
- 1 Elastic IP per private IPv4 address (Remove the public IPv4 and replaces with the elastic IP. This will completely lose that dynamic IP and will be different if you had to remove the Elastic IP)
- 0 or more IPv6 addresses
- Security groups
- Source/Destination check

### Notes

- Secondary ENI + MAC = can be used for licensing 
- Multi-homed (subnets) management & data
- Different Security Groups you will need multiple interfaces
- Operating System - **Doesn't** see the public IPv4 address
- IPv4 Public IPs are *dynamic* (stop/start = change)
- Public DNS = **private IP in VPC**, public IP everywhere else