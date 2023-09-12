---
title: 01f - Organizations
tags:
  - aws
---

## What are they?

The problem is there are situations where an organization would have to manage multiple AWS Accounts. This becomes a management issue.

The solution is you take a standard AWS account that is not within an Organization and create a new organization. The organization is not in this account, it is just used to create it. This then become the management account for this organization (*Management / Master Account*).

This master account can then invite other AWS accounts to join that organization.

The Organization and all its standard accounts fall under the Organization Root (*this is not a root user, it is just a container*). It then allows you to create what is called *Organization Units (OU)*.

What is useful with Organizations is that you can centralize the billing in the Master Account, or Payer account. This has number of benefits outside of management, such as consolidation of reservations and volume discounts.

## How to create an organization

1) Log into your general account, that is *NOT* your root user
2) Click on top right menu and click organization
3) Create organization (you may need to verify an email)
4) Once you have your organization you can then invite

## Role Swapping with pre-existing accounts

When you create roles from within your organization then a role is automatically created for that account, which can be role switched into from other accounts in that org. If you invited pre-existing accounts then you need to manually create this role.

### Creating a role for your pre-existing account

1) Go to your account that you have invited and head to IAM
2) Go to roles on left hand nav
3) Choose AWS Account Role
4) Fill in the AWS account you want to allow, in this case your management account ID
		![[Pasted image 20230912123204.png]]
5) Hit next, then make sure you give *Admin Access*, then hit next
6) Give a Role Name *OrganizationAccountAccessRole* (this is just a standard name that AWS would do automatically when creating within an org. this is just for consistency)
7) Create Role

This will create a new role with the trust relationship to your management account ID

![[Pasted image 20230912123648.png]]

### Swapping roles from your management account

1) From top right drop down click switch role
2) Click Switch Role
3) Using the account ID you want to switch to paste in the Account
4) Enter the role you want to switch to (*OrganizationAccountAccessRole*)
5) Enter Display Name and Color you want
6) This will allow you to switch back and forth between roles

This provides temporary credentials to that account role we just made. This is great for switching easily between accounts that have provided access.


### Creating an account within your organization

1) From organization click *add account*
2) Select create AWS Account
3) Enter credentials and create
4) You can now switch to this new account

## Service Control Policies

Are a feature of AWS Organizations which allow restrictions to be placed on MEMBER accounts in the form of boundaries.

SCPs can be applied to the organization, to Organizational Units (OU's) or to individual accounts.
SCPs *DON'T GIVE* permission - they just control what an account *CAN* and *CANNOT* grant via identity policies.

Note: The Management Account is never affected by SCP. You should generally avoid using your management account for AWS Resources or in general. Just use it for account management in your org.

The overlap of permission policies and SCP's is as follows:

![[Pasted image 20230912142017.png]]