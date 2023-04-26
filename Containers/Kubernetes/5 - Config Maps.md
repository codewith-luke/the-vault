Similar to secret stores you can also create centrally stored configs (Centrally store data).


## Using Config Maps

To get exisiting config maps run:

```sh
kubectl get configmap
```

To create a new config map

```sh
kubectl create configmap {name} --from-literal=app.{key}={value}
```

You can then view the results with:

```sh
kubectl get configmap -o yaml
```

You can also create the configmap with a file:

```sh
kubectl create configmap {name} --from-file={file}
```

## Mounting Config Maps

Similar to a secret file or env setup (see [[4 - Secrets#Mounting Secrets in Containers]]) You can use a file to then specify the configs.

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: configmap-pod
spec:
  containers:
    - name: test-container
      image: nginx
      volumeMounts:
      - name: config-volume
        mountPath: /etc/config
  volumes:
    - name: config-volume
      configMap:
        name: dev-propertieshttps://github.com/zealvora/certified-kubernetes-administrator/blob/master/Domain%203%20-%20Services%20and%20Networking/nodeport.md
  restartPolicy: Never
```

Which you can then run:

```sh
kubectl apply -f {file}
```

