---
title: 01e - IAM Roles
tags:
  - aws
---
## What are IAM Roles?

It is a type of *identity* that exists within an AWS account (this is a different identity to a user). 

Generally speaking when it comes to a IAM User, it is a 1-to-1, person that uses a single IAM User.
A role is a bit different, it is 1-to-many. It would be multiple AWS users, applications etc. 

Roles are generally also done on a temporary access, it is used short term to use it's permissions, then stop being that role.

Roles can be used within AWS organizations to access different accounts without having to log in again.

![[Pasted image 20230911123202.png]]

## Types of Policies

IAM Roles have 2 types of policies that can be attached:

- **Trust Policy**
	- Which identities can assume this role
	- Can reference identities in same account (IAM users/roles and services)
	- Can reference identities in other AWS accounts
	- If something is given access, AWS generates *temporary security credentials*, this is done by an AWS service called **STS or Secure Token Service**, and are made available to the identity which assumed the role. Think of them like access keys, but time limited.
- **Permissions Policy**
	- Based on the trust policy giving security credentials, the identity will now have access to the permissions specified within the permission policy.

![[Pasted image 20230911124157.png]]

## When to use IAM Roles?

- If you do not know the amount of [[@Terms#Principal]] who need access, roles are the ideal.

- AWS Services (e.g. AWS Lambda)
	- If you did not use a role here you would need to hardcode permissions into the lambda function. You should generally avoid this. This is a security and rotation issue.
	- This goes back to first point as well, you do not know how many lambda's may be used.
		![[Pasted image 20230911130857.png]]

- Emergency role. This is a *break the glass* sort of emergency situation. 
		![[Pasted image 20230911131501.png]]

- Adding AWS into an existing corporate environment.
	- This is useful if you have a lot of staff (> 5000)
	- When you want to reuse existing identities for use within AWS. 
		- The reason for this is external accounts can't be used in AWS directly. e.g. Microsoft Active Directory cannot be used directly in AWS.
		![[Pasted image 20230911131839.png]]

- You have an application with a lot of users (e.g. Uber) that needs to interact with resources.
		![[Pasted image 20230911132133.png]]

- Cross account access.
		![[Pasted image 20230911132401.png]]

## Service Link Roles & PassRole

AWS Service Linked Roles are a type of IAM (Identity and Access Management) role that allows AWS services to interact with resources in your account. These roles are pre-defined by AWS and are designed to be used only by AWS services. Unlike general IAM roles, which you can create and modify, the permissions for service-linked roles are managed and maintained by AWS.

#### Key Features:

1. **Predefined**: AWS creates these roles for you, and they come with the necessary permissions that the service will need.
2. **Immutable**: You cannot modify the permissions attached to these roles, ensuring that the service has exactly the permissions it needs and no more.
3. **Automatic**: In many cases, the service-linked role is automatically created for you when you activate a particular AWS service.
4. **Account-specific**: Each service-linked role is tied to your AWS account and is used to perform actions only within that account.
5. **Secure**: Because you can't modify the permissions, there's less risk of accidentally granting too much access.

#### Use Cases:

- Enabling EC2 instances to call other AWS services on your behalf.
- Allowing AWS Lambda to access an S3 bucket.
- Permitting AWS Glue to write logs to CloudWatch.

### PassRole

The `PassRole` permission allows you to delegate permissions to AWS services that need to create and manage AWS resources on your behalf. Essentially, it allows one service to "pass" an IAM role to another service. This is often necessary when you're setting up services that need to interact with each other.

#### Key Features:

1. **Delegation**: Allows an IAM user to pass a role to an AWS service, granting that service the permissions defined in the role.
2. **Scoped**: You can specify which roles can be passed and to which services, providing fine-grained control over permissions.
3. **Explicit**: You must explicitly grant `PassRole` permissions; they are not granted by default.
4. **Secure**: Helps in maintaining a least-privilege security posture by only allowing specific roles to be passed to specific services.

#### Use Cases:

- Allowing an EC2 instance to assume a role that has permissions to access an S3 bucket.
- Granting AWS CloudFormation the ability to create a Lambda function with a specific execution role.

In summary, Service Linked Roles are predefined roles used by AWS services to interact with your account, while `PassRole` is a permission that allows you to delegate role-passing capabilities to services or users. Both are essential components in managing permissions and interactions between AWS services.