---
title: 01g - Control Tower
tags:
  - aws
---
## What is it?

AWS Control Tower offers a straightforward way to set up and govern an AWS multi-account environment, following prescriptive best practices. AWS Control Tower _orchestrates_ the capabilities of several other [AWS services](https://docs.aws.amazon.com/controltower/latest/userguide/integrated-services.html), including AWS Organizations, AWS Service Catalog, and AWS IAM Identity Center (successor to AWS Single Sign-On), to build a landing zone in less than an hour. Resources are set up and managed on your behalf.

AWS Control Tower orchestration extends the capabilities of AWS Organizations. To help keep your organizations and accounts from _drift_, which is divergence from best practices, AWS Control Tower applies preventive and detective controls (guardrails). For example, you can use guardrails to help ensure that security logs and necessary cross-account access permissions are created, and not altered.

### Quick Points 

- Quick and Easy setup of multi-account environments
- Orchestrates other AWS services to provide this
	- Organization, IAM Identity, CloudFormation, Config and More
- Most of the time you would mostly interact with the Landing Zone - multi-account environment
- Provides Guard Rails - Detect/Mandate rules/standards across all accounts
- Account Factory - Automates and Standardizes new account creation
- Utilizes IAM Identity Center (AWS SSO) - SSO, Multiple-accounts, ID Federation

![[Pasted image 20230912160257.png]]

### What are Guard Rails

- Are rules for multi-account governance
- Mandatory, Strongly Recommended or Elective types

### Types of Guard Rails:

- **Preventative**:  to stop you doing things via SCP
	- These are either *enforced* or *not enabled*
	- i.e allow or deny regions or disallow bucket policy changes
- **Detective**: Compliance check via AWS Config Rules
	- These are either *clear*, *in violation*, or *not enabled*
	- i.e. detect CloudTrail enabled or EC2 Public IPv4

In short preventative stops and detective identifies.

## What is Account Factory

- Automated Account Provisioning
	- Cloud admins or end users with appropriate permissions
- Applies guardrails automatically
- Account admin given to a named user via IAM Identity Center
- Accounts & network are provisioned with *standard configuration*
	- This avoids overlap 
	- And is good for accounts at scale
- It allows accounts to be *closed* or *repurposed*
- Can be fully integrated with a business SDLC