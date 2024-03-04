---
title: 06b - Elastic Container Service
tags:
  - aws
---
## What is it?

This is when you accepts containers and instructions your provide  and is run on within AWS (fully or partially). Just means less work for you to manage.

## How it works?

ECS let's you create a cluster. Clusters are where you containers run from. You provide it an image and it runs from within the cluster. 

First you need a way to tell ECS about container images that you want to run and how. These containers would be located on a registry somewhere (Dockerhub/ECR (Elastic Container Registry)/etc). 

1) To tell ECS about your container images, you make a **container definition**. It tells ECS where your container is. [Learn about Container Definiton](https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_ContainerDefinition.html)

- Define image and ports

2) Then to represent a self contain application you have **task definitions**. A task could have one or many containers in it. A task in ECS represents the application as a whole. This could be one or more containers. [Learnt about Task Definition](https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_TaskDefinition.html)

- Security (Task Role), Container(s), Resources
- Task Role - IAM role which the task assumes

3) You then have a **service definition**. This describes how your application should scale and availability.

- How many copies, High Availability, Restarts

## ECS Cluster Types

There are 2 modes

- EC2 Mode
- Fargate Mode

### EC2 Mode

In this you can specify the amount of instances you want and the AZ that they are provisioned in. 

With EC2 cluster mode you are responsible for these EC2 instance that are acting as container hosts.

You need to worry about capacity and availability for your cluster. You will be paying for anything running. ECS will take some of that management overhead but is still more of a middle ground to managing your cluster by yourself.

![[Pasted image 20240213084428.png]]
### Fargate Mode

This is a cluster model. In this you would have no service to manage. You are not paying for EC2 instances. It will use same surrounding technologies as EC2 mode, difference is you don't manage this and how it is hosted.

This is done through a shared infrastructure. You gain access to resources from a shared pool, with no visbility to other customers.

This infrastructure is then injected into a VPC that is based off your configuration. At this point it works just like any other VPC resource.

![[Pasted image 20240213084858.png]]

## When to use these?

- If you use container use *ECS*
- Large workload + price conscious = *EC2 Mode*
- Large workload + overhead conscious = *Fargate*
- Small / Burst workloads = *Fargate*

## Deploying container to Fargate Cluster

1. Go to Elastic Container Service
2. Go to clusters on left and create cluster
	1. Enter your name
	2. Select your VPC or use the default as this is configured already
	3. Fargate infra should already be selected
	4. Create
3. Go to task definitions and create a new one
	1. Put the name
	2. Set the container details
	3. Input the docker image for this container
	4. Go next
	5. Choose the OS (Linux/X86_64)
	6. Choose CPU (.5 vCPU)
	7. Uncheck use log collection if not needed
	8. Go next
	9. Create after overview
4. Go to clusters
5. Select the your cluster and go to tasks tab
6. Run new task
	1. Select **launch type** under environment
	2. Ensure Fargate is selected under launch type drop down
	3. Under deployment configuration make sure application type is **Task**
	4. Under family select your container
	5. Under networking ensure your vpc  and subnets(default in this case is selected)
	6. Create new security group and make it relevant
		1. Select type HTTP
		2. Source as anywhere (so anyone can access it)
	7. Turn on public IP
	8. Click create
7. To remove stop the container
	1. Go to task definitions and actions to deregister
	2. Go to clusters and your cluster and delete


