---
title: 02g - High Availability + Fault Tolerance +Disaster Recovery
tags:
  - aws
---
## What is **High Availability**?

Aims to ensure an agreed level of operational performance, usually uptime, for a higher than normal period. 

A common misconception of *High Availability* is that things that are highly available do not go down, or there is zero downtime. This is not correct.

It is one designed to be online as often as possible. When failure does happen the system is built in such a way that it is able to bring itself back online (often through automation). It is about maximizing a systems online time, and that's it. If there is minor user disruption then that is considered acceptable. Only when outages occur does this become a problem.

There is something called *nines* where it is the amount of downtime that SLA and systems can be offline. For example:

- *Three 9 (99.9%)* = 8.77h per year downtime
- *Five 9 (99.9%)* = 5.26m per year down time

## What is **Fault Tolerance**?

People often mix *High Availability* with *Fault Tolerance*.
It is the property that enables a system to continue operating properly in the event of the failure of some (one or more faults within) of its components.

This means that if a system has faults then it should continue to operate properly even when these faults are present. So it has to **operate through a failure.**

## What is **Disaster Recovery**?

A set of policies, tools & procedures to enable the recovery or continuation of a vital technology infrastructure and systems following a natural or human-induced disaster.

*HA & FT* are about creating systems that are able to cope through disaster. Disaster recovery is about planning for and what to do when the above do not work? 

This is a multi-stage set of processes on what needs to be done. This is about understanding where to find, how to access and what responsibilities need to be handled and what processes need to be followed.


### Summary

- High Availability - Minimize any outages
- Fault Tolerance - Operator through faults
- Disaster Recovery - Processes when the above don't work