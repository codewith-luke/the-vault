Instead of storing your credentials hardcoded. It is recommended to create a Central Secret Store. This will then allow your applications to fetch these credentials and not hardcode these directly within the pod.

An example of a central store would be AWS Secret Manager or Hashicorp vault.

## To get existing secrets

The following will list all secrets currently available:

```sh
kubectl get secret
```

```sh
kubectl get secret {name}
```

## To create a secret

```sh
kubectl create secret generic {name} --from-literal=password=my-password
```

In the aboce example `--from-literal=password=my-password` is creating a key value pair of `password=my-password`

You can also create from a file:

```sh
kubectl create secret generic {name} --from-file=secret-data.txt
```

## See output of a Secret

To see more details about a secret you can set the output as YAML:

```sh
kubectl get secret {name} -o yaml
```

This will output something to the likes of:
```YAML
apiVersion: v1
data:
  password: bXktcGFzc3dvcmQ=
kind: Secret
metadata:
  creationTimestamp: "2022-12-04T14:08:47Z"
  name: my-secret
  namespace: default
  resourceVersion: "1234"
  selfLink: /api/v1/namespaces/default/secrets/my-secret
  uid: abcdef01-2345-6789-abcd-ef0123456789
type: Opaque
```

Where password as per our example when creating the secret is a base64-encoded string which you would have to decode yourself.

## Mounting Secrets in Containers

Once a secret is created, it is necassary to make it available to containers in a pod.

There are 2 approaches:

1. Volumes
2. Env variables

#### Volume Example

```YAML
apiVersion: v1
kind: Pod
metadata:
  name: secretmount
spec:
  containers:
  - name: secretmount
    image: nginx
    volumeMounts:
    - name: foo
      mountPath: "/etc/foo"
      readOnly: true
  volumes:
  - name: foo
    secret:
      secretName: firstsecret
```

#### Env Example

```sh
apiVersion: v1
kind: Pod
metadata:
  name: secret-env
spec:
  containers:
  - name: secret-env
    image: nginx
    env:
      - name: SECRET_USERNAME
        valueFrom:
          secretKeyRef:
            name: firstsecret
            key: dbpass
  restartPolicy: Never
```

**With the environment variable approach the secret is not encoded so you will not have to go through that extra step of decoding.**

### Useing Secret Files

You can then simply apply either of the above example:

```sh
kubectl apply -f {file}
```

Then when connecting to that pod you will be able to connect as it references a secret that is within the cluster.