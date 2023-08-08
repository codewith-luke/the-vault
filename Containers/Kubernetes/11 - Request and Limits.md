If you schedule a large application in a node which has limited resource, then it will soon lead to memory issues or possible downtime.

Request and Limits are 2 ways we can control the amount of resources that can be assigned to a Pod.

An example of a YAML file with Request and Limits would look something like:

```YAML
apiVersion: v1
kind: Pod
metadata:
  name: nginx-pod
spec:
  containers:
  - name: nginx-container
    image: nginx
    resources:
      requests:
        memory: "64Mi"
        cpu: "0.5"
      limits:
        memory: "128Mi"
        cpu: "1"
```

So this will now ensure when creating this Pod that it will assign it to a node with the correct amount of resoources available to do so.

To learn more on what would be available use: 

```sh
kubectl describe node {node}
```

**Important to note that in terms of the primary concern with regards to scheduling Requests availability is taken into consideration first**