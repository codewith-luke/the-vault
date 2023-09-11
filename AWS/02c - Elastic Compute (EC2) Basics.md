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

### Connecting to EC2

EC2 instances support *Windows* or certain distros of **Linux**. 

Windows uses the *Remote Desktop Protocol* (RDP), which runs on *port 3389* for windows.
For Linux this uses the *SSH Protocol*, which runs on *port 22*. This you would need an SSH key pair.

When you create an EC2 instance you decide on using a previous or create a new key pair. The private part is only available once (*you need to keep this safe*). The public key would be placed on the instance.
