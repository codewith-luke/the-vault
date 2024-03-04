---
title: 007 - Advanced EC2
tags:
  - aws
---
## EC2 Bootstrapping

- Allows for bootstrapping (creating) and EC2 Build automation
- It is enabled by using User Data - Accessed via the meta-data IP
	- http://169.254.169.254/latest/user-data
- Anything in User Data is executed by the instance OS
	- Only on launch
- EC2 doesn't interpret, the OS needs to understand the User Data, so it just passes in the data for the instance to understand.

### User Data Key Points

- It is opaque to EC2, it's just a block of data
- It is not secure - not to be used for passwords or long term credentials
- Can not be > 16KB, anything bigger would require a script to download
- Can be modified when the instance is stopped
- Contents are only executed at launch
	- Generally used for post-launch configuration of an instance


#### Boot-Time-To-Service-Time

There are a few ways for it to be done:

![[Pasted image 20240219085348.png]]

## How to

1. Create your EC2 Instance
	1. Select your VPC
	2. Select appropriate subnet
	3. Auto assign IP
	4. Select your security group
2. Scroll down to advanced details and look for user data input and put your user data (start-up logic) into the input
3. Launch instance

To see the metadata on the instance:

```
TOKEN=`curl -X PUT "http://169.254.169.254/latest/api/token" -H "X-aws-ec2-metadata-token-ttl-seconds: 21600"`

curl -H "X-aws-ec2-metadata-token: $TOKEN" -v http://169.254.169.254/latest/meta-data/

curl -H "X-aws-ec2-metadata-token: $TOKEN" -v http://169.254.169.254/latest/user-data/
```

To view the system logs you can go to `cd /var/log` this can allow you to see any bootstrapping issues or other log types.