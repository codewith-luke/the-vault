# Table of Content

[[1 - Docker Compose]]
[[2 - Docker Swarm]]

Orchestration is about managing life-cycles of containers in dynamic environments.

Some things orchestration can do is:

- Provision and deploy containers
- Scaling up or removing containers to spread application load
- Movement of containers from one host to another based on resource availability
- Load balancing of service discovery between containers
- Health monitoring - 0 -  of containers and hosts

## Docker Swarm

This is a container orchestration tool which is natively supported by docker. These are called *swarm clusters*.

To get started with Swarm we will be working with Droplets (VMs) on Digital Ocean. In our case we have created 3 VM's that you will have to ensure all are updated and have docker installed.

In order for swarm nodes to communicate with each other these are done over an *overlay network* see [[6 - Overlay Network]].
