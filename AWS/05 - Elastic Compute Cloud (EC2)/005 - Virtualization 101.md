---
title: 005 - Virtualization 101
---
#### Links
[http://www.brendangregg.com/blog/2017-11-29/aws-ec2-virtualization-2017.html](http://www.brendangregg.com/blog/2017-11-29/aws-ec2-virtualization-2017.html)

## What is it?

Virtualization is the process of running more than one OS on a piece of physical hardware (server). 

![[Pasted image 20231130084523.png]]

The problem with early virtualization is this was inefficient. This was due to the hardware not being aware of this virtualization and so when these multiple operating systems needed privileged access it would cause issues.

### Emulated  Virtualization

This was where **Emulated Virtualization** came into play. This included new capability called **hypervisor**. The host operating system. Then each of the other operating systems would act as virtual machines on their own operating systems. These would act as purely software and not interact with hardware directly (which when multiple OS did caused issues). All hardware is "fake" to make the virtual machines believe it was interacting directly to the hardware. When reality is it was via the **hypervisor**. It does this over what is called *binary translation*. 

![[Pasted image 20231130085114.png]]

The above however was not performant and there was another way to achieve this.

### Para-Virtualization

The main difference here is that instead of using *binary translation* it would only work with a small subset of operating systems. So these generic operating systems are modified to then make specific calls directly to the **hypervisor** rather than over the poor performing binary translation method.

![[Pasted image 20231130085437.png]]

This improved performance, but it was still just software talking to software and tricking the operating system to think it is in fact interacting with hardware.

### Hardware Assisted Virtualization

As the name suggests this is now where the hardware itself becomes aware of virtualization. So this would mean if the virtual machine was interacting with the CPU, the CPU is aware that it is performing virtualization.

So what will happen is the virtual machines would interact directly with the hardware but in fact it the hardware would redirect this responsibility the the **hypervisor**.

![[Pasted image 20231130085834.png]]

### SR-IOV (Single Route IO Virtualization)

It allows a network card on the host to present itself as mini cards to the virtual machines. As this is supported in hardware these are unique cards and are presented to the VM's as real cards. And so the VM's would interact directly with this.

In **EC2** this is called *Enhanced Networking*. This improves performance massively and consistent.

![[Pasted image 20231130090226.png]]