---
title: "@Basic EC2 Template"
tags:
  - aws
---
## What is it?

- Helper script (**cfn-init**) installed on EC2 OS
- But more than that, it is a simple configuration management system
- *Procedural* (user data) vs *desired* state (cfn-init)
- Can make sure packages, groups, users, sources, files, commands and services are setup/installed.

![[Pasted image 20240221084626.png]]