---
title: 07b - EC2 Instance Roles
tags:
  - aws
---
## How it works

- Credentials are inside the meta-data
	- In iam/security-credentials/role-name
- Automatically rotated
- Should always use roles where possible than adding access keys to an instance
- CLI tools use the ROLE credentials automatically
- Go [here](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html#cli-configure-quickstart-precedence) to understand configuration settings and precedence

![[Pasted image 20240222083623.png]]

## Creating EC2 Instance Roles

1. Create your instances (or stack)
2. Go to IAM console and Roles and create a role
3. Select AWS service and give permission policies you want
4. Give your role name and create (this would create your role and your instance profile if done via the UI)
5. Go to your instance right click, go to security and then modify the role with your new role
6. Connect to your instance and you should be able to use the below `aws s3 ls`
	1. You can view your credentials with the below curl commands

```
aws s3 ls

curl http://169.254.169.254/latest/meta-data/iam/security-credentials/

curl http://169.254.169.254/latest/meta-data/iam/security-credentials/A4LInstanceRole
```