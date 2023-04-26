Kubernetes was built to run on distributed systems where than can be hundres of worker nodes in which Pods would run.

This makes networking a very important aspect. It allows admins to properly run, monitor as well as troubleshoot applications in k8 clusters.

Kubernetes imposes some fundamental requirements on any networking implementation:

1. Pod on a node can communicate with all pods on all nodes without NAT
2. All nodes can communicate with all Pods without NAT
3. The UP that pod sees itself as is the same IP that others see it as.

## Challenges and Solutions

Based on the contstraints set there are 4 different networking challenges that need to  be solved.

- Container to Container Networking
	- Primarly happens  inside a POD
	- Pods can contain a group of containers with same IP address.
	- Communication between the containers inside pods happens via localhost

- Pod to Pod Networking
- Pod to Service Networking
	- K8s service can act as an abstraction which can provide a single IP address and DNS through which pods can be access (see [[6 - Service]])
	- Endpoints track the IP address of the objects that service can send traffic too.

- Internet to Service Working
	- This can be solved using K8 Ingress. This is a collection of routing rules which govern how external users access the services running within the k8 cluster.

## Network Policies

By default pods are non-isolated. They accept traffic from any source.

This is where policies come in. They determine how groups of pods are allowed to communicate with each other and other network endpoints.

A good use case its lets say you have some pods running and one gets compormised. You would then want to isolate it and prevent communication happening to it.

```YAML
apiVersion: networking.k8s.io/v1
kind: NetworkPolicy
metadata:
  name: my-network-policy
spec:
  podSelector:
    matchLabels:
      app: {pod}
  policyTypes:
  - Ingress
```

To understand the 2 types of policies there is Ingress and Egress.

-   "Ingress" traffic is incoming traffic to the selected Pods.
-   "Egress" traffic is outgoing traffic from the selected Pods.