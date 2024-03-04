---
title: 05g - Instance Status Checks and Autorecovery
tags:
  - aws
---
## What is it?

Status checks have 2 checks

- System status
- Instance status

![[Pasted image 20240205085058.png]]

### Create Status Check Alarm

1. Go to your instance
2. Click and head to the status checks tab
3. Click on actions and then create a new status check alarm
	- Here you can configure to **recover/reboot/stop/terminate**
	- Can configure EC2 to create brand new instances on a terminate, but not from this menu

### Termination Protection

1. Go to your instance and right click to go to *instance settings*
2. *Change termination protection* and then enable
3. 