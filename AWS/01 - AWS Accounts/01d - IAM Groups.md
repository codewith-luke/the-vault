---
title: 01d - IAM Groups
tags:
  - aws
---

## What are Groups?

They are an admin or container feature. In an exam you may get a trick question asking if you can log into a group. You *cannot*.

Groups are *NOT* real identities... 
They can't be used from resource policies and have no credentials to login with.

An IAM User can be part of multiple groups. They are an effective way to organize users and their perms. 

Groups can of course have policies (*inline/managed*). 

If you are part of multiple groups, AWS will merge any policy permissions from those into one. Including if you have inline within a group.

![[Pasted image 20230911120120.png]]

The same *Allow and Deny* rules will apply. So if you gather up all the policies and permissions, things like explicit deny are still taking preference.

Another trick question is around an *all group*. There is no such thing in AWS. Users without a group, have no groups. 

## Summary

- 300 Groups per account (can be increased with a ticket)
- Can't be logged into
- Allow/Deny rules still apply with multiple policies across groups and inline
- Groups are *not* a *true identity*. They can't be referenced as a [[@Terms#Principal]] in a policy. 
	  - An example of this would be with resource policy you can actually reference a user or a role. This is not the case with groups.
