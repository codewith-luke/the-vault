---
title: 05f - EC2 Purchase Options
tags:
  - aws
---
## On-Demand

- On-Demand instances are isolated by *multiple customer instances* run on shared hardware.
- Instances of different sizes run on the same EC2 Hosts - consuming a defined allocation of resources
- **Per Second Billing** while an instance is running.
- Associated resources like *storage* consume capacity, so bill regardless of the instance state.

#### When to use 

- Default purchase option so good to evaluate
- Predictable
- No interruption
- No capacity reservation
- No upfront cost
- No discount
- *Short term* workloads
- *Unknown* workloads
- Apps which can't be interrupted

## Spot

- SPOT pricing is AWS selling unused EC2 host capacity for *up to 90% discount* - the spot price is based on the spare capacity at a given time.
- Spot instance is like bidding. So if you set a max price for a spot instance at $2 and AWS decides that instances are now $2.1 then you instances will go away. However if you had it set to $3 then you would not be affected.

#### When to use

- Never use SPOT for workloads which can't tolerate interruptions
- Used for non-time critical
- Anything which can be rerun
- Burst capacity needs
- Cost sensitive
- Anything stateless

## Reserved

- Long term usage of an EC2
- Means a reduced or no price per second cost
- Unused reservation still billed
- Partial coverage of larger instance
- 1y or 3y terms
- *No-upfront* - this means a reduced per second fee
- *Partial Upfront* - smaller per second but you pay a small upfront amount
- *All upfront* - whole instance fee, greatest discount
#### When to use

- You know you need it long term
- You know you need certain amount of resources
- When you want reduced costs

#### Schedule Reserved Instances

- Scheduled is ideal for long term usage which *doesn't* run constantly
	- E.g. Weekly data, sales analysis every Friday for 24h
- Doesn't support all instance types or regions
- Have to have 1200 hour per year & 1 year term minimum

#### Capacity Reservations

- Ensure you always have access to *capacity in an AZ* when you need it
- But at full on-demand price
- Has no term limits, but you pay regardless of if you consume it.

#### EC2 Savings Plan

- An hourly commitment for *1 || 3* year term
- A reservation of *general compute $ amounts* ($20 per hour for 3 years)
	- Or a specific EC2 Savings plan - flexibility on size & OS
- Compute products currently EC2, Fargate & Lambda
- Products have an on-demand rate and a savings plan rate
- Resource usage consumes savings plan commitment at the reduced savings plan rate
- Beyond your commitment on demand is then used
## Dedicated Hosts

- Paying for the host itself
- You can expect what you would get with your own. Dedicated cores etc
- All instances on the host are not charged, but you have to manage it.
- Has something called host affinity, links instances to hosts

#### When to use

- When you have software that is licensed to sockets/cores

## Dedicated Instances

- Your instances run on an EC2 host with other instances of yours, no other customers use the same hardware
- You don't own or share.
- Extra charges for instances but dedicated hardware
- One off hourly fee for any regions where you are using dedicated instances regardless how many
- Fee for instance itself

#### When to use

- When you cannot share infrastructure with others

![[Pasted image 20240202090551.png]]