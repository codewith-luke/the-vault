Taints are used to repel pods from specific nodes.
So for example if you have a worker node that has a specific taint. It will then repel the request from that specific pod.

Whereas if another worker does not then it will go through:

![[Pasted image 20221205171420.png]]

To schedule a pod with a tain you make use of **Tolerations**. You can consider these as a special pass to allow it.

To find if a specific node has a Taint use:

```sh
kubectl describe node {name}
```

Then scroll down to Taint key and that will show you info you need.

To then add a taint to a node you can use:

```sh
kubectl taint nodes {node} key=value:NoSchedule
```

This means if you had to create Pods they would be assigned to the node that doesn not have a Taint.

If you wish to create your Pods with tolerations as your pass you would add the following to your YAML:

```YAML
tolerations:
-key: "key"
operator: "Exists"
effect: "NoSchedule"
```

This would match to checking `key` exists and its value is `NoSchedule`.

To remove a taint from the node use the same command but add a `-` to the end.

```sh
kubectl taint nodes {node} key=value:NoSchedule-
```