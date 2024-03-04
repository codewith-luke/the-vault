---
title: 04b - Building a custom VPC
tags:
  - aws
---
## What is it?

- [Tool to calculate ranges for subnets](https://www.site24x7.com/tools/ipv4-subnetcalculator.html)

Custom VPC as the name suggests is a custom VPC network that allows you to have more control and configure your VPC.

VPC as we know allows nothing IN or OUT without explicit configuration. 
A custom VPC allow flexible configuration (*simple* or *multi-tier*) as well as hybrid networking, allowing you to connect to other cloud platforms.

When creating a VPC you have the option of selecting *DEFAULT* or **Dedicated Tenancy**. This controls whether the resources on the VPC are provisioned on shared hardware or dedicated hardware. *BE CAREFUL WITH THIS*. 

If you choose *DEFAULT* then you can choose on a per resource basis whether it goes on shared hardware or dedicated hardware later on. If you pick  **Dedicated Tenancy** at a VPC level then that is locked in (This comes at a cost premium). Unless you really know you need dedicated, just choose default.

### Summary Points

- Custom VPC's can use IPv4 Private CIDR blocks & public IP's. By default it uses the private, public is for when you want to make a resource public.
- It is allocated 1 primary private IPv4 CIDR Block
	- Smallest min */28 (16 IP)* and max */16 (65 536 IP)*
	- You can add optional secondary IPv4 blocks
- Can be configured to use *IPv6 /56* CIDR Block 
	- You can't pick a block like IPv4, you either have to let AWS decide or use your own list of IPv6 addresses
	- They also do not have the concept of public or private, but still means you just configure how you want
- AWS VPC's have fully featured DNS by Route 53
	- It is available inside the VPC (VPC `Base IP + 2` address)
	- e.g 10.0.0.0 => DNS IP 10.0.0.2
	- There a 2 options for configuring how DNS works in a VPC
			- `enableDnsHostnames` - gives instances DNS names. If true, instances do get public DNS hostnames
			- `enableDnsSupport` - enables DNS resolution in VPC. 
			- These should be the first things you check when you having issues in a VPC

## What we will be building

- NOTE: Make sure to checkout the [[04a - VPC Sizing and Structure Process#Proposal]] and the IP plan before proceeding. 

![[Pasted image 20231016152022.png]]

The above is going to be doing the following:

- Creating a VPC across 3 AZ's
- Split into 4 tiers running in 4 AZs which is 16 possible subnets
	- In the diagram the 4th subnet is for future AZ
- We will also be creating an internet gateway and a NAT gateway as well as a bastion host.
	- NOTE: Bastion is not best practice and is generally frowned upon, but shown what not to do and that there are more secure alternatives

## How to create your VPC

1. Head to VPC
2. Click create VPC
	- You can choose between *VPC* and *VPC and More*, to go through the whole process select *VPC*
3. Give you VPC a name
4. Add the CIDR range (i.e. something like 10.16.0.0/16)
5. Select *Amazon-provided IPv6 CIDR block* to enable IPv6
6. Click create
7. By default because this is a custom VPC it will not have any subnets inside, we have to do that.
	1. To make sure we do not have any issues head to your VPC and Edit VPC settings
	2. Make sure *Enable DNS Resolution* and *Enable DNS Hostnames* are enabled and save

## How to create multi-tier subnet VPC

1) Head to VPC and go to subnets (make sure you have done [[#How to create your VPC]])
2) Select your VPC you created and then in the subnet settings put the name of your first subnet (i.e. sn-reserved-A)
	1) Enter the CIDR range (10.16.0.0/16)
	2) Then enter the CIDR block (10.16.0.0/20)
	3) Select IPv6 Range
	4) Add new subnet and repeat for your subnet
	5) Create subnet (If you are following the above you should have a total of 12 subnets across 3 AZ's)
3) Once you have created your subnets make sure to enable IPv6 auto allocate, this can be done by editing each subnet and enabling it.

This whole above process would normally be done via automation. So it is just good to know how to do it manually.

