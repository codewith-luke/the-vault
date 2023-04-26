https://github.com/zealvora/certified-kubernetes-application-developer/blob/master/Domain%202%20-%20POD%20Design/labels.md
Labels are key balue pairs atached to objects such as pods. They are great for identifying and running commands based on labels.

```
name: gateway
env: production
```

With the above we can see an example of 2 labels. With a key of name/env and value of gateway/production.

To then search existing pods for your label you can use:

```sh
kubectl get pods -1 env=dev
```

### Seeing Details of a POD

If you want to see detailed info about a pod use:

```sh
kubectl describe pod {name}
```

The `kubectl describe pod` command provides detailed information about a specific Kubernetes pod.

To show the labels of a pod you can then use:

```sh
kubectl get pods --show-labels
```

This will give you something along the lines of:

```sh
NAME                             READY   STATUS    RESTARTS   AGE    LABELS
my-app-5b55c8b8f6-mgfhj          1/1     Running   0          5d     app=my-app,release=stable
my-app-5b55c8b8f6-qrq9k          1/1     Running   0          5d     app=my-app,release=stable
my-app-5b55c8b8f6-rhrl9          1/1     Running   0          5d     app=my-app,release=stable
```

As you can see we have labels `app=my-app` and `release=stable`.


### Add a new label

To then add to a new label to our scenario above:

```sh
kubectl label pod my-app-5b55c8b8f6-rhrl9 tier=frontend
```


### Filter Labels

Which then allows you to filter your labels:

```sh
kubectl get pods -l tier=frontend
```

This will find all pods besides the specified:

```sh
kubectl get pods -l tier!=frontend
```

### Remove label

```sh
kubectl label pod my-app-5b55c8b8f6-rhrl9 tier="" --overwrite
```