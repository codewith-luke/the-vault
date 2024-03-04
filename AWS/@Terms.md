
## Principal

A principal is **a human user or workload that can make a request for an action or operation on an AWS resource**.

## Identity Policy

These are permission and access policies. You can read more here [[01b - IAM Identity Policies]]
## Resource Policy

Resource Policies are resource allow/deny rules. Similar to [[#Identity Policy]] but specific to resources. They come with a number of benefits:

- Resource policies ALLOW/DENY same or different accounts
	- This grants the ability to grant other accounts access to resources inside of your account
- They can also ALLOW/DENY Anonymous principals
- The come with an *explicit* [[#Principal]] field. It shows who this applies to. In the case below this is a * which is anyone. So this could mean anyone, internal identities, partner accounts, anonymous.

![[Pasted image 20230914085226.png]]

## Choosing between Resource and Identity Policies

- Identity: Controlling different resources
- Identity: You have a preference for IAM
- Identity: Same account
- Resource: Just Controlling a resource (S3)
- Resource Anonymous or Cross-Account

## DHCP

Stands for *Dynamic Host Configuration Protocol*. It is a network management protocol used to dynamically assign an IP address to any device, or node, on a network so it can communicate using IP
