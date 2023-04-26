## Liveness Probe

Many applications running for long periods of time eventually transition to broken states. K8 provides liveness probes to detect and fix such situations.(Replica)[[2 - Replica Sets]]

Essentially think of it as a watcher over your pods and then managing and restarting them.

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: liveness
spec:
  containers:
  - name: liveness
    image: ubuntu
    tty: true
    livenessProbe:
      exec:
        command:
        - service
        - nginx
        - status
      initialDelaySeconds: 20
      periodSeconds: 5
```

The above is an example of creating a container with `livenessProbe` that would then execute commands that if ever returned an error would then restart that container.

## Readiness Probe

It can happen that an application is running but temporarily unavailable to serve traffic.

For example your application is running but its still loading its large config files from an external vendor. In such cases we dont want ti kill the container however we also do not want it to serve the traffic.

![[Pasted image 20221205164621.png]]

So if we look at the following example we have two pods running. If one is not ready the load balancer will not distribute traffic to it and rather allow the one that is able to accept.

You will have to define what determines that the readiness is available. If we look at the below example:

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: readiness
spec:
  containers:
  - name: readiness
    image: ubuntu
    tty: true
    readinessProbe:
     exec:
       command:
       - cat
       - /tmp/healthy
     initialDelaySeconds: 5
     periodSeconds: 5
```

The readiness probe set here will only be ready if we have a file healthy in the tmp folder. This means if it is not there our pod(Replica)[[2 - Replica Sets]] will not allow traffic.