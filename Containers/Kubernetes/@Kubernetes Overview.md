# Table of Content
[[1 - Labels and Selectors]]
[[2 - Replica Sets]]
[[3 - Deployments]]
[[4 - Secrets]]
[[5 - Config Maps]]
[[6 - Service]]
[[7 - Networking]]
[[8 - Liveness and Readiness Probe]]
[[9 - DaemonSets]]
[[10 - Taints and Tolerations]]
[[11 - Request and Limits]]

Kubernetes (k8s) is an orchestration engine by Google.

Similar to Docker swarm master node. Kubernetes would create a master node with various worker nodes.

There are 3 ways to install K8s:

- Managed K8s service (Digital Ocean, AWS, etc.)
- Minikube (Does not provide everything)
- Manual Installation (Harder)

## Installing kubectl

https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/

### Helpful Refs

```sh
kubectl api-resources

kubectl explain {resource}
```

## Connecting to K8 Master

To connect to the K8s master there are 2 things needed:

- DNS/IP
- Auth Creds

## Creating Pods

```sh
kubectl run {name} --image={image}
```

### Connecting to a POD

```sh
kubectl exec -it {name} -- bash
```

## Kubernetes Objects

Pods are an example of an Object. There are other instances such as namespace, deployments and so on, they are not just pods.

There are various ways to configure an Object.

- `kubectl`
- Config file in YAML

#### Multiple Object Types in a Kubernetes Cluster

1.  Pods
2.  Deployments
3.  ReplicaSets
4.  Services
5.  ConfigMaps
6.  Secrets
7.  DaemonSets
8.  StatefulSets
9.  Ingress
10.  Jobs
11.  CronJobs

### Example POD YAML

To create run `kubectl apply -f {filename}.yaml`
To delete run `kubectl delete -f {filename}.yaml`

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: nginxwebserver
spec:
  containers:
  -  image: nginx
     name: democontainer
```