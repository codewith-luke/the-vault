## Public vs Private Services in AWS

AWS Services can be divided into public and private AWS services.

In traditional sense when we think of public vs private, public may be considered something such as public services like GMAIL or Youtube. Whereas private you may be familiar with something like your personal home network.
### Private
AWS also has it's own *private zones*. This are called a **VPC** ([[02b - Virtual Private Cloud Basics (VPC)]]) What these allow is for nothing externally to access unless configured. You can place things like *EC2* instances.

### Public
AWS then also has a *public zone*. This runs between the public internet and between *private zones*. It is a zone that is connected to both. This is the zone that AWS public services would operate from, think *S3*.

![[Pasted image 20230827123341.png]]

## AWS Global Infrastructure

[https://www.infrastructure.aws/](https://www.infrastructure.aws/)

### AWS Regions and Edge Locations

Regions are geographically spread. Which means we can use these to avoid global level disasters. 
Regions have a **Region Code (like ap-southeast-2)** and a **Region Name (Asia Pacific (Sydney))**.

This spread means that when you interact with *Elastic* in Virginia it is different than the one in Sydney.

**Regions have 3 main benefits:**
- Geographic separation - Isolated fault domain
- Geopolitical Separation - Different governance (*EU vs US*)
	- You generally have to tell AWS that you are OK with data travelling between regions
- Location Control - Performance
#### Availability Zones (AZ)

Inside every region there are multiple **availability zones**. These are isolated infrastructure inside of  a region, this means isolated *compute, storage, networking, power & facilities* within a region. 

This means if a zone is affected by an outage, it would mean the other AZ's would likely be unaffected. This means you can spread your infrastructure within a region across AZ's.

![[Pasted image 20230827125215.png]]
#### Service Resilience

- **Globally Resilient** - means a service that is spread across multiple regions across AWS. This would take the whole world to fail for a full outage to occur (*IAM, Route53*).
- **Region Resilient** - Operate as separate services in each region. They generally replicate data across AZ's.
- **AZ Resilient** - Run from a single AZ. If the zone fails, then that service fails.
#### Edge Locations

Edge locations are much smaller than regions, but are a lot more of then, and generally only contain content distribution services. These are useful for people like Netflix who need to store data close to their customers. With this split a large company may run their infrastructure from a few regions, but spread their content across lots of different edge locations. 
