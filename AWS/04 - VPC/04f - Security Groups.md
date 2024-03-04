---
title: 04f - Security Groups
tags:
  - aws
---
## What are they?

Security Groups (SGs) are another security feature of AWS VPC ... only unlike NACLs they are attached to AWS resources, not VPC subnets.

SGs offer a few advantages vs NACLs in that they can recognize AWS resources and filter based on them, they can reference other SGs and also themselves.

But.. SGs are not capable of explicitly blocking traffic - so often require assistance from NACLs.

### Key Points

- Stateful - detect response traffic automatically
	- So an *allowed* (in or out) *request* = *allowed response*
- They do not have a explicit deny. Only allow or implicit deny
	- So they cannot be used to block bad actors
	- This is why using this with a NACL is common
- Support IP/CIRD based rules and logical resources
	- Including other security groups and itself
- They are not attached to instances
	- Are attached to ENI (Primary network interface)


## Logical References

When you have 2 or more applications that you want to apply a SG you are able to make use of references to other security groups. These are known as logical references. 

For example if you had a web and an app instance, where your web instance allowed traffic in over TCP from any IP. You may decide to have a security group that would then allow this. Your app instance could then make use of a *reference* to your SG on the web instance.

![[Pasted image 20231116084038.png]]

This then means it we do not have to worry about IP addresses or CIDR ranges and scales really well.

## Self References

An SG can also reference itself. As an example this means if you have multiple instances and they make use of a SG that has a self reference then communication between these instances is open to one another.

![[Pasted image 20231116084609.png]]

This simplifies things like intra app communication. Or communication **from** instances that have that SG attached **to** instances that have that SG attached.