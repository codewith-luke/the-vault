---
title: 01 - AWS Accounts
tags:
  - aws
---
## What is an AWS Account?

An AWS Account is a container for **identities (users)** and **resources**.

For an AWS account you need to have a unique email and credit card. As we think of this as a container, this is where the expenses would filter up from the other identities and resources.

When creating an account you will then have a **root user** that can only login to that AWS Account. The root user will always have full control and access. This root account is super important as it is the controlling factor.

**Important:** 
- By default all access externally to an AWS account is denied. Unless configured otherwise.
- When creating an account make sure to do the following:
	- Go to Account
	- Scroll down to "IAM user and role access to Billing information"
	- Enable this
	This is because by default your IAM users will not be allowed access to billing information. By enabling this, as long as they have permissions to view, they can now see billing info.

![[Pasted image 20230822084814.png]]

### How to setup MFA

1) Account
2) Security Credentials

![[Pasted image 20230823085815 1.png]]
3) Complete process

### Setting up a budget
For [Free Tiers](https://aws.amazon.com/free/) checkout the following.

1) Go to top right
2) Billing Dashboard
3) Go to left hand side *Preferences* => *Billing Preferences* 
	- Enable all the options (besides legacy) and fill in any info to get updates
4) Goto Cost management => Budgets
5) Create a budget
	- Stick to template and choose between zero/monthly and fill in data
## What is IAM?

*IAM* or Identity and Access Management, this is a **No Cost** service. Allows you to create *users, groups and roles* for an AWS account. These will always start with no permissions but then they can then be given full or limited permissions for that AWS Account.

You can give permission to identities these can be:
- Users
- Applications

**IAM** is a globally resilient service, so will always be secure. It will always be separate and is a dedicated instance to your AWS account.

It has full authorisation (permissions) the account and account root user has.
#### What can you create?

- Users
	- **Identities** which represent **humans** or **applications** that need access to your account
- Groups 
	- **Collection** of related users eg. dev team, finance, HR
- Roles
	- Can be used by **AWS Services**, or for **granting external** access to your account

#### What is an IAM Policy?

These are essentially documents that *allow* or *deny* access to AWS services. They do nothing on their own. But when attached to a *User, Group or Role* will determine what can be done.

#### IAM's Responsibilities

IAM has 3 main jobs

1) An IDP (ID Provider)
	- This is creating users, groups, roles 
2) Authenticate
	 - This is about proving who you say you are (like a username and password) 
3) Authorize
	- This is about allowing your or denying your based on policies set.

![[Pasted image 20230824084909 1.png]]

##### In summary

- No cost
- Global service / Global resilience
- Allow or Deny its identities on its AWS account
- No direct control on external accounts or users
- Identity federation and MFA

### Creating an IAM Identity


##### Create Account

**Prerequisites**:

- Navigate to the search bar and look for `IAM` service

Here you can see the dashboard and you can optionally set an *alias* for your account. This must be globally unique. It is recommended to do this so you can easily get to your login page and prefill the *Account ID* information when logging in

![[Pasted image 20230825142335.png]]


1) Left hand menu click on users
2) Create User
	- For your first admin user make sure to  give access to AWS Management Console.
3) Choose the User Type
4) Give permissions. Here you can choose existing groups or copy perms
	- If none configured use Attach Policies Directly
	- To give admin use `AdministratorAccess	AWS managed - job function`
5) Complete the user create and then close down and return to user list
6) You should now head back to IAM dashboard and go to your login alias URL you have set earlier and login with your new account.

##### Securing your IAM User

1) Head to Security Credentials
2) Assign MFA
3) Relog to validate MFA works

## IAM Access Keys

- Username and password
- Access Keys

These are considered as *long term credentials*. These are considered long term as they do not regularly change, like changing a password or access key.

The advantage/disadvantage for a user identity is that it can only have one username and password. You could consider the public part of the login the *username* and the private part *password*.

The difference with access keys is an **IAM user can have 2 access keys**. No more than that.

Access keys can be created/delete and make active/inactive.

### Creating Access Keys

1) Head to security scroll down and then click access keys
2) Choose what type of access key
3) Create the name for your key your want.
4) Download the .csv details
5) Once created you can now manage your key you have created

**Install the CLI:**
AWS CLI Install - https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html

##### Configuring CLI

1) Run `aws configure`
	- This will setup the default configuration profile, you can also setup named profiles
	- To create with a profile run `aws configure --profile {name}` 
2) Enter from your downloaded .csv creds
3) Enter a default region *i.e. us-east-1*
4) Enter format, else just hit enter
5) You should now be able to use something like `aws s3 ls --profile {name}`






