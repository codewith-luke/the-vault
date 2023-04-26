A ReplicaSet purpose is to maintain a stable set of replica Pods running at any time. Similar to a [[2 - Docker Swarm]]

## Listing Replica Sets with `kubectl`

To list replica sets using `kubectl`, you can use the `kubectl get` command with the `replicasets` subcommand. For example, to list all replica sets in a cluster, you can use the following command:

```sh
kubectl get replicasets
```

This command will list all replica sets in the cluster, along with their names, images, and number of replicas.

## Filtering Replica Sets by Label

You can also use labels to filter the replica sets that are listed by the `kubectl get` command. For example, to only list replica sets that have the `app: nginx` label, you can use the following command:

```sh
kubectl get replicasets -l app=nginx
```

This command will only list replica sets that have the `app: nginx` label. You can specify multiple labels to filter the replica sets even further. For example, to only list replica sets that have both the `app: nginx` and `environment: production` labels, you can use the following command:

```sh
kubectl get replicasets -l app=nginx,environment=production
```

## Displaying Labels in the Output

You can also use the `--show-labels` option to display the labels of each replica set in the output of the `kubectl get` command. For example, to list all replica sets and their labels, you can use the following command:

```sh
kubectl get replicasets --show-labels
```

This command will list all replica sets in the cluster, along with their names, images, number of replicas, and labels.

## Creating a Replica Set with `kubectl`

To create a replica set using `kubectl`, you can use the following command:

```sh
kubectl create replicaset <replica-set-name> --image=<image-name> --replicas=<number-of-replicas>
```

For example, to create a replica set called `my-replica-set` with 3 replicas of the `nginx` image, you would use the following command:

```sh
kubectl create replicaset my-replica-set --image=nginx --replicas=3
```

You can also use the `kubectl apply` command to create or update a replica set. To do this, you would create a `ReplicaSet` object in a YAML file and then pass the file to the `kubectl apply` command, like this:

```sh
kubectl apply -f replicaset.yaml
```

Here is an example of a `ReplicaSet` object in YAML:

```yaml
apiVersion: apps/v1
kind: ReplicaSet
metadata:
  name: my-replica-set
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

This `ReplicaSet` object will create a replica set with 3 replicas of the `nginx:1.7.9` image.