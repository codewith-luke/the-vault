---
title: 02k - Systems Manager Parameter Store
tags:
  - aws
---
## What is it?

- it is a public service
- Storage for *configuration* & *secrets*
	- Can store String, StringList & SecureString
- Can store things like Licence codes, Database Strings, Full Configs & Passwords
- Has Hierarchies & Versioning
- Can also store Plaintext and Ciphertext (for encrypting with [[03e - Key Management Service (KMS)]])
- Has public parameters - *i.e. Latest AMIs per region*

![[Pasted image 20240222085338.png]]