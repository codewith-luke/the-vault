DaemonSet can ensure that all Nodes run a copy of a Pod. This is helpful when new nodes are added that these pods are added as well. An example is adding an antivirus to new nodes.

These are setup quite similar to a [[2 - Replica Sets]]

```YAML
apiVersion: apps/v1
kind: DaemonSet
metadata:
  name: kplabs-daemonset
spec:
  selector:
    matchLabels:
      name: kplabs-all-pods
  template:
    metadata:
      labels:
        name: kplabs-all-pods
    spec:
      containers:
      - name: kplabs-pods
        image: nginx
```

To then view DaemonSets use:
```sh
kubectl get daemonset
```

Then to get more info on it use:

```sh
kubectl describe daemonset {name}
```
