---
title: 04a - VPC Sizing and Structure Process
tags:
  - aws
---
- [AWS Amazon VPC Connectivity Options](https://d1.awsstatic.com/whitepapers/aws-amazon-vpc-connectivity-options.pdf)
- [Understanding IP address ranges](https://www.hava.io/blog/what-is-cidr-notation#:~:text=The%20%E2%80%9C%2F16%E2%80%9D%20CIDR%20notation,first%2016%20binary%20bits%20match.)
## Considerations when creating a VPC

- The IP range (The IP plan). This is something you should think of in advance, as it is difficult to change.
- What *size* should the VPC be (how many services or things can be inside this VPC)
- Are there any other networks we *can't* use
- Being mindful about other ranges of other VPC's, Cloud, On-premises, Partners & Vendors
- Try predict what could change in future
- Consider the structure of a VPC - Tiers and Resiliency (AZ)

## VPC Scenario

Let's take an example. Say we are working with  a system that has 3 head offices, so we know we need *3 IP address ranges*. We don't know what the networks are yet, but we can find these things out. 

We also know there will be workers going to our various services, it is up to us to ask the questions on how they may access these systems (Through site, VPC etc).

![[Pasted image 20231012084001.png]]

### IP Ranges to avoid

Based on what we already know of the 3 existing IP ranges. We know we have to avoid them.

![[Pasted image 20231012084156.png]]

These are confirmed networks that are already in use. Now during our questions we may have asked we may discover that there are some other on-prem networks in use. As well there is an unknown network in Google cloud. But we do know the default range. In this case it is a huge range.

![[Pasted image 20231012084412.png]]

When creating our business plan this is our starting point. We now know what ranges are and what to avoid.

### Some more considerations

- VPC minimum **/28 (16 IPs)**, maximum of **/16 (65536 IPs)**
- Some people have a personal preference on range (*eg 10.x.y.z*)
- Avoid common ranges (*eg 10.0 or 10.1*)
- Reserve 2+ networks per region being use per account
	- e.g. 3 US, Europe, Australia - is 5 total so we want to make 2 networks per region. Which is 10 ranges - We would assume 4 AWS Accounts
	- Total *40* ranges (ideally)

#### VPC Sizing

![[Pasted image 20231012085332.png]]

##### Questions to ask when selecting a size?

- How many *subnets* will you need?
- How many *IPs*? How many *per subnet*?

## What is a Subnet?

Subnets are what services run from inside a VPC. They provide structure, functionality and resilience to VPC's.

Subnets start off as private, they require some config to become public.

*NOTE:* When it comes to colouring of subnets in diagrams *blue* represents a private subnet while *green* is public.
### Key Points

- AZ resilient feature of a VPC
- A subnetwork of a VPC - within a particular AZ
- 1 Subnet => AZ, 1AZ => 0+ Subnets.
	- 1 subnet in 1 AZ. A subnet can never be in more than one AZ. But an AZ can have 1 or more subnets
- Assigned a IPv4 CIDR and is a subset of the VPC CIDR
	- Cannot overlap with other subnets
	- Can optionally be allocated a IPv6 CIRD (*/64* subset of the */56* VPC - space for 256)
- Subnets can communicate with other subnets in a VPC 
- There are 5 reserved IP addresses in a subnet
	- So lets say we have 10.16.16.0/20 (10.16.16.0 => 16.16.31.255)
		- *Invalid* Network address (10.16.16.0)
		- *Invalid* Network+1 (10.16.16.1) - Used by the VPC router
		- *Invalid* Network+2 (10.16.16.2) - Reserved (DNS*)
		- *Invalid* Network+3 (10.16.16.3) - Reserved for future use
		- *Invalid* Broadcast Address (10.16.31.255) - The last IP in subnet
- A VPC has a [[@Terms#DHCP]] option set applied to it
	- There is one of these applied to a VPC and this flows through to subnets
	- It controls things like DNS servers, BIOS servers etc.
- You can define 2 important IP allocation options on a subnet
	- Auto assign public IPv4
	- Auto assign IPv6
### Deciding Subnets

You can't just use a VPC to launch services into, in AWS services use subnets where IP addresses are allocated from. VPC services run from within subnets *not* the directly in the VPC.

A subnet runs within an availability zone, so the first decision you need to make is how many AZ you will need. This depends somewhat on the region as some regions have 3 or more. The best option is to start with 3 as your default, and you should try always add a spare, so *4 AZ*. This is the assumption of a Web, App, DB and a spare for future use.

If you think of this as a grid going over these AZ per layer. This would then come to a total of *16 subnets*.

So if we chose a */16* for the VPC, it would mean each of the 16 subnets would need to fit into that */16*. This means a */16*  VPC split into 16 subnets results in 16 smaller networks ranges each of which is a */20*. 

How did we get to */20*? 

This is because each time the prefix is increased from */16 => /17* it creates 2 networks then from */16 => /18* is 4 then */16 => /19* is 8 then finally */16 => /20* is 20 smaller networks. Basically whatever prefix you choose for the VPC, the subnet will be 4 steps away.

## Proposal

When defining the IP plan for the business, we need to assume a huge level of growth.

- As we need know the IP ranges we need to avoid, we could use the *10.16 -> 10.127* range (avoiding google).
- So with this in mind for our regions.
	- US1 - start at 10.16
	- US2 - 10.32
	- US3 - 10.48
	- EU - 10.64
	- AUS - 10.80
- Each AWS account has a *1/4th*
- /16 per VPC - 3AZ (+1), 3 Tiers (+1) - 16 Subnets
- /16 split into 16 subnets = */20* per subnet (4091 IPs)
- [IP Addressing plan here](https://github.com/acantril/aws-sa-associate-saac02/tree/master/07-VPC-Basics/01_vpc_sizing_and_structure)