---
title: 05i - Instance Metadata
tags:
  - aws
---
## What is it?

- Is a service that EC2 provides to instances by providing data to those instances
- Information about the environment that it would not be able to access otherwise
- Accessible inside all instances
- The IP to access the instance metadata is http://169.254.169.254/latest/meta-data
	- This allows you to query any information about that instance (like environment, networking, authentication)
- Used to pass in temporary SSH keys
- Handles user-data
- Has no authentication and is not encrypted (can be blocked with local firewalls, but is extra overhead, treat is as public)
