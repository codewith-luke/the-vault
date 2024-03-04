---
title: 04c - VPC Routing and Internet Gateway
tags:
  - aws
---
## What is it?

Every VPC has a VPC Router (highly available) and is on every subnet *network+1* address. The role is to route traffic between subnets. Which is controlled by 'route tables' and each subnet has one.

A VPC is created with a *main route table* - subnet default. A subnet can only be associated with one route table at a time. But a route table can be associated to many subnets.

![[Pasted image 20231101085309.png]]
## Internet Gateway

- *Region resilient* gateway attached to a VPC
- 1 VPC = 0 or 1 IGW, 1 IGW = 0 or 1 VPC
	- Meaning an IGW can only be attached to 1 VPC
- IGW runs within the AWS public zone
	- Gateways traffic between the VPC and the internet or AWS Public Zone (S3, SQS, etc)
- Managed by AWS

![[Pasted image 20231101085831.png]]

### IPv4 Addresses with an IGW

- *Important:* in IPv4, the public IP is not configured on the OS. It is a record handled on the gateway. Public IP never touches your EC2 instance.

![[Pasted image 20231101090039.png]]

The flow of this means that when a packet goes from our instance our IGW will change the source to the *public* IP address and then ensure that it sends it on. This is also true of the inverse.

![[Pasted image 20231101090257.png]]

## Bastion Host / Jumpbox

- Bastion Host = Jumpbox
- It is an instance in a public subnet 
- That handles manages incoming connections
- Then access internal VPC resources
- This is often the only way *IN* to a VPC


## Creating an Internet Gateway

1) Go to VPC and then Internet Gateways on the left
2) Click create internet gateway and enter your name then create
3) Click on actions and then attach to your existing VPC
4) On left head to route table
5) Click create a new route table
	1) Enter your name
	2) Select your VPC
	3) Create
6) Head over to Route tables and then select your route table and go to subnet associations tab
7) We now need to associate our web subnets with this route table
	1) Click on edit associations
	2) Select all your public facing subnets
	3) Save associations
8) Go to routes tab for us to add some new routes (default for IPv4 and default for IPv6)
	1) Click add route
	2) Enter `0.0.0.0/0` (means all IP's, anything IPv4)
	3) Under target select gateway and your new gateway we created earlier
	4) Then add a new routes `::/0` (This is for IPv6 default)
	5) Save changes
9) Head back to subnets and ensure all your subnets you want public then have auto assign IPv4 address configured under the subnet settings (edit the subnet to do this)