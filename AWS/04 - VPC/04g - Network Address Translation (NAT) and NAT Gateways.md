---
title: 04g - Network Address Translation (NAT) and NAT Gateways
tags:
  - aws
---
## What is it?

It is a set of processes which can adjust IP packets, by changing their source or destination IP addresses. 

When people think of NAT a lot of them think of *IP masquerading*, this is the concept of hiding CIDR blocks behind one IP. Rather than one private to one public IP process we see in internet gateways, NAT is many private IP to single public IP. This approach is popular as IPv4 addresses are running out.

It gives private CIDR range to outgoing internet access.

AWS has 2 ways that you can traditionally do NAT. There is 

- EC2 Service
- AWS NAT service

### Basic NAT Architecture

![[Pasted image 20231123084537.png]]

## When do you need a NAT Gateway?

- If you need to give an instance it's own public IPv4 address then only an **internet gateway** is required.
- If you are wanting to give private instances outgoing access to the internet and AWS public zone services like S3 then you will need **internet gateway** AND **NAT Gateway**.

## Key Points

- Needs to run from a public subnet
	- Requires you to have an Internet gateway, subnets configured to allocate public IPv4 address and default routes
- Uses **Elastic IP's** (static IPv4 public)
- AZ Resilient Service
	- To achieve region resilience you need a NAT gateway in each AZ
	- Then a route table for each AZ with that NAT gateway as the target
- Are a managed service
	- Scales to 45Gbps
	- $ Duration (hourly charged) and Data volume (Per Gb)

## Example Architecture

The following example will give us a truly resilient system. It is about making it available across AZ and region resilient and scalable.

![[Pasted image 20231123085821.png]]

##  NAT Gateway vs NAT Instance (as EC2 Instance)

![[Pasted image 20231123085840.png]]

*Important* - If you choose to use a NAT instance you need to ensure your disable *source/destination* checks.

## What about IPv6?

- NAT isn't required for IPv6
- All IPv6 addresses in AWS are publicly routeable
- Internet Gateway works with ALL IPv6 IPs directly
- NAT Gateways *don't work with IPv6*
- `::/0` (default IPv6 route) + IGW for bi-directional connectivity
- `::/0` (default IPv6 route) + Egress-Only Internet Gateway - Outbound only