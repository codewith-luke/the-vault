---
title: 02c - Elastic Compute (EC2) Basics
tags:
  - aws
---

## What are they?

- EC2 is **IAAS** (Instance As A Service) - Provides virtual machines (instances).
- Private service by default - uses **VPC** networking
- AZ Resilient - Instance fails if AZ fails
- Can choose instance *sizes* and *capabilities*
- Offers on demand billing - *Per second*
	- CPU
	- Storage
	- Extras - Commercial software the instance is launched with
- Local on-host storage or Elastic Block Store (**EBS**)

#### EC2 Instance Lifecycle

- Running
	- Will be *billed fully* on
		- CPU
		- Memory
		- Storage
		- Networking
- Stopped
	- Will be *billed partially*
		- Storage
- Terminated
	- Will *not* be *billed*

### Amazon Machine Image

An **AMI** can be used to create an EC2 instance. Or you can create an AMI from an EC2 instance. 
Think of these things as server images to create new images. Almost like templates for EC2 instances.

- AMI contains attached permissions
	- This could be set to public if you didn't want to restrict
	- Can be set to only the Owner
	- Explicit - this would be for specific AWS accounts
- Contains the **Root Volume**
- Has the **Block Device Mapping**. :Think of this as a mapping between volumes and how the operating system views them.

### Methods of Connecting to EC2

EC2 instances support *Windows* or certain distros of **Linux**. 

Windows uses the *Remote Desktop Protocol* (RDP), which runs on *port 3389* for windows.
For Linux this uses the *SSH Protocol*, which runs on *port 22*. This you would need an SSH key pair.

When you create an EC2 instance you decide on using a previous or create a new key pair. The private part is only available once (*you need to keep this safe*). The public key would be placed on the instance.


## Creating an EC2 Instance

1) Go to EC2 dashboard
2) Create a SSH key value pair if one does not exist
	- Left hand side scroll down to Network & Security and look for Key Pairs
	- Create keypair (PEM is for most modern OS's)
3) Go to instances on left, then click launch Instances
4) Choose whatever instances you want (in our case free tier compat)
5) Choose your key-pair you want to use
6) With network settings you can also adjust here (if you click *Edit* you can change things like VPC, Subnet etc.)
7) Setup the Security Group name you want under network settings
8) Scrolling down we can also configure storage (for us will leave as default)
9) Launch instance when done
10) This will then put the instance into pending and doing setup work, wait for this (status check needs to change).

### Connecting to new EC2 Instance

1) Click on your new instance
2) Click connect and you can see all options to connect 
3) Click SSH client and it will give you the steps to connect