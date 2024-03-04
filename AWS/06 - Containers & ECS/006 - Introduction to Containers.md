---
title: 006 - Introduction to Containers
tags:
  - aws
---
## What is it?

When it comes to instances a lot of the storage can be taken up by the OS. It is not uncommon to see something like the below, in terms of how instances might be taken up:

![[Pasted image 20240209083821.png]]

However when using containers this becomes a little bit different where you would have your container engine above your host OS:

![[Pasted image 20240209084113.png]]

This means we can share rather than duplicate. This way when interacting with the host it is via the docker engine layer and so does not require each instance to run it's own OS.

## Image Anatomy

The basic anatomy of a Docker image is made up of multiple layers. This as an example could look something like (Make sure to checkout [[4 - Images Instructions]]):

![[Pasted image 20240209084525.png]]

So based on an image a Docker Container can just be viewed as a running instance based off of an image. This container comes with an additional layer, the *Read/Write* layer.