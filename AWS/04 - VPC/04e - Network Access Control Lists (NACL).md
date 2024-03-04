---
title: 04e - Network Access Control Lists (NACL)
tags:
  - aws
---
## What is it?

A _network access control list (ACL)_ is an optional layer of security for your VPC that acts as a firewall for controlling traffic in and out of one or more subnets. You might set up network ACLs with rules similar to your security groups in order to add an additional layer of security to your VPC. This lesson steps through the features of a NACL, the impact of their stateless nature and some of the key points to be aware of for the exam.

This can be thought of as a traditional firewall in AWS VPC. They are *stateless -* [[04d - Stateful and Stateless Firewalls#Stateless Firewall]]. NACL are associated with subnets. So each subnet will have an NACL. This then filters data as it crosses the boundary of that subnet. 

However it is important to remember, things within a subnet do not get affected by that NACL. It is only external

When it comes to the diagram below an important note is that rules are processed in order, as well as an *asterix*  in the below case means that it has a deny if nothing else matches.

![[Pasted image 20231109085847.png]]

A good example of a ruleset is as follows:

![[Pasted image 20231109090313.png]]

Then a more complicated understanding when we have communication between subnets:

![[Pasted image 20231109090553.png]]

### Important points

- Stateless - *Request* and *Response* are seen as different
- Only impact *data crossing subnet boundary*
- NACLs can *EXPLICITLY ALLOW* and *DENY* (meaning you can block IP's and ranges)
- NACL are not aware of logical resources (IPs/CIDR, Ports & Protocols)
- NACLS cannot be assigned to AWS resources, only *subnets*
- Use together with **Security Groups** to add explicitly DENY 
- Each subnet can one *one NACL* (Default or custom)
- A NACL can be associated with *many subnets*