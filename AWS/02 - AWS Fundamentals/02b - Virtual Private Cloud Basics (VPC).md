---
title: 02b - Virtual Private Cloud Basics (VPC)
tags:
  - aws
---

## What are VPC's?

As the name suggests there are virtual private network inside AWS. A VPC is *1 account* & *1 region*.
*VPC* is private and isolated unless you say otherwise. 

There are *2 types* of VPCs.

- Default  (**Can only have one Default per region!**)
- Custom (**Can have multiple**)

In custom deployments you are likely to use custom VPCs. Where default come preconfigured in a very specific way, and all the networking is done on your behalf, as a such they are a lot more restricting.

They can are used to create:

- private networks in AWS that other private services will run from
- and connect AWS private networks to create private on premises networks when creating a hybrid environment. 
- a service that allows you to connect to other cloud platforms when creating a muiti-cloud deployment.

## Default VPC

*Every* VPC is given a range of IP ranges (**VPC CIDR**). Anything communicating *in* needs to communicate to that VPC CIDR. Custom VPC's can have multiple VPC CIDR while the default VPC always gets **one that is always (172.31.0.0/16).**

A VPC can provide resilience in that it can sub-divided into subnets across AZ's. Each subnet can be split into one AZ and is set on creation and can't be changed. Default is preconfigured to have one subnet in every AZ.

When split into an AZ it will use the range of the VPC CIDR. These cannot be the same as other subnets in the VPC and can't overlap with other subnets in the VPC. The IP ranges of the subnets also define the **Start** and End **IP** addresses which any private services in those subnets will use.

![[Pasted image 20230827134141.png]]

#### Summary
- One per region - can be removed & recreated
- Default VPC is always 172.31.0.0/16, same predictable structure
- In each VPC each /20 subnet IP range in each AZ in the region
- Default provides a Internet Gateway (IGW), Security Group (SG) & Network ACL (NACL)
- Subnets assign public IPv4 addresses (preconfigured by default)

