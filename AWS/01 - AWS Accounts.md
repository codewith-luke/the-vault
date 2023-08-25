
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

![[Pasted image 20230823085815.png]]
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

![[Pasted image 20230824084909.png]]

#### In summary

- No cost
- Global service / Global resilience
- Allow or Deny its identities on its AWS account
- No direct control on external accounts or users
- Identity federation and MFA




