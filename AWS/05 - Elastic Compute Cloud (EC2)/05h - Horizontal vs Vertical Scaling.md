---
title: 05h - Horizontal vs Vertical Scaling
tags:
  - aws
---
## Vertical Scaling

Means scaling size of an instance, more powerful resources.

- Each resize requires a reboot - *disruption*
- Larger instances often carry a *$ premium*
- There is an upper cap on performance - *instance size*
- No application modification required
- Works for all applications - even monoliths

## Horizontal Scaling

This is just taking your amount of instances or copies, you run multiple.

- Requires some form of load balancer
- Session management is important
	- You would need to make sure session management is not managed on an instance
	- Or *off-host sessions*
- Allows for no disruption when scaling
- No real limits to scaling
- Often less expensive - no large instance premium
- More granular in how you scale

