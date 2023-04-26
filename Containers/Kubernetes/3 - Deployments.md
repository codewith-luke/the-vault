Deployments provides replication functionality with help of ReplicaSets. These are things like rolling out changes or rollbacks and being able to choose which rollbacks you want to use. 

These are done in such a way that it ensures that the exisitng application does not get shut down. If we take our previous replica set YAML example [[2 - Replica Sets#Creating a Replica Set with `kubectl`]] . We modify the `kind` to `Deployment` and the name to make it easier.

```YAML
apiVersion: apps/v1
kind: Deployment
metadata:
  name: my-deployment-set
spec:
  replicas: 3
  selector:
    matchLabels:
      app: nginx
  template:
    metadata:
      labels:
        app: nginx
    spec:
      containers:
      - name: nginx
        image: nginx:1.7.9
        ports:
        - containerPort: 80
```

You can then run `kubectl apply -f deployments.yaml` and this will then create it.

To view deployments use:

```sh
kubectl get deployments
```

## Rolling Out Changes

This will create a new replica set with new pods and once it is running correctly it will then remove the previous.

First you would have to make chages to your YAML for it to pick up changes.

Once done you can then re-apply.

### Describe A Deployment

To get details on a deployment use:

```sh
kubectl describe deployments {name}
```

#### Rollout History

```sh
kubectl rollout history {name}
```

To the further view a specific revision and its change:

```
kubectl rollout history {name} --revision 1
```

## Max Surge and Max Unavailable

`maxSurge`: Maximum number of PODS that can be scheduled above original number of pods.
`maxUnavailable`: Maximum number of pods that can be unavailable during the update.
