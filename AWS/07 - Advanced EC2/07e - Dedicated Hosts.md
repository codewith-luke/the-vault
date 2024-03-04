---
title: 07e - Dedicated Hosts
tags:
  - aws
---
## What is it?

Dedicated hosts are EC2 Hosts which support a certain type of instance which are dedicated to your account.

- Specific family eg. a1, c5, m5
- No instance charges, you pay for the host
- On-demand and reserved options available
- Host hardware has physical socket and cores

Generally dedicated hosts are used for applications which use physical core/socket licensing

[https://aws.amazon.com/ec2/dedicated-hosts/pricing/](https://aws.amazon.com/ec2/dedicated-hosts/pricing/)

### Limitations & Features

- AMI Limits - RHEL, SUSE Linux and Windows AMIs aren't supported
- Amazon RDS instances not supported
- Placement groups are not supported
- Hosts can be shared with other ORG accounts...**RAM**
