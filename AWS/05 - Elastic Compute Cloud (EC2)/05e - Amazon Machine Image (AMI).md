---
title: 05e - Amazon Machine Image (AMI)
---
## What is it?

An Amazon Machine Image (AMI) in AWS is a pre-configured virtual machine image that contains the necessary information to launch and run an instance in the Amazon Elastic Compute Cloud (EC2).

- Can be AWS or Community Provided AMI's
- There is also Marketplace AMI (can include commercial software. comes generally with extra cost)
- Are regional (different *unique ID* per region)
- AMI also controls permissions (by default set to only your account, but this can be changed)

## AMI Lifecyle

1. Launch
2. Configure
3. Create Image
4. Launch

![[Pasted image 20240201084517.png]]

## Useful Notes

- AMI - *One Region*, only works in that one region
- *AMI Baking* - Is creating an AMI from an already configured instance + application
- An AMI *can't be editied*. To "edit" you need to launch and instance, update the config and remake the AMI
- Can be copied between regions
- Permissions are controlled by the AMI (default = your account) 

## Creating an AMI

1. Shut down your  instance if it running (this can cause consistency issues)
2. Right click your instance and under **Image and templates** select **create image**
	1. Enter information for your AMI
	2. Create
3. Go to AMI once it is ready
4. Right click you AMI and *launch instance from AMI*
5. Configured your instance and launch
	- Make sure your auto assign for IP is set
6. Once it is created you should now be able to connect with your correct user

## Copying and Sharing an AMI

1. Head to region with your AMI
2. Select copy AMI and your new region
3. The complete your copy

## Edit AMI Permissions

-  Right click your AMI and edit permissions (default is your user)