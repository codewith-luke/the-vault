(Replica)[[2 - Replica Sets]]When you create a Pod you will have a relavant Private IP address. 

So a K8 service can act as an abstraction which can provide a single IP address and DNS through which pods can be accessed.

This layer of abstraction allows us to perform a lot of operations like `load balancing`, `scaling` and others.

## Creating an example service

https://github.com/zealvora/certified-kubernetes-administrator/blob/master/Domain%203%20-%20Services%20and%20Networking/serviceandendpoints.md

```sh
kubectl run backend-pod-1 --image=nginx
```

Lets make another pod:

```sh
kubectl run backend-pod-2 --image=nginx
```

And then a frontend

```sh
kubectl run frontend-pod --image=ubuntu --command -- sleep 3600
```

Then we can run the following to see our outputs:

```sh
kubectl get pods -o wide
```

### Creating our Service

Now that we have our pods running we can create our service:

```yaml
apiVersion: v1
kind: Service
metadata:
  name: my-service
spec:
  type: ClusterIP
  ports:
    - port: 8080
    targetPort: 80
  selector:
    app: my-service
```

We can then start up our service with:

```sh
kubectl apply -f {file}
```

Now that you  have your service run:

```sh
kubectl get service
```

You can then get the IP of your new service. Now right now we have nothing utilizing this service. To do that we need to assign our backends we just created to our new created service.

So below we have created a new Endpoint Yaml file where we specify the IP addresses for the various endpoints we have.

```yaml
apiVersion: v1
kind: Endpoints
metadata:
  name: my-service
subsets:
  - addresses:
    - ip: {IP}
    ports:
	    - port: 80
```

We can then apply this:

```
kubectl apply -f {file}
```

Once this is done you can then connect to your frontend and make a query to the service and this will use your assigned pods.

## Different Types of Services

### ClusterIP
Whenever a service type is `ClusterIP`, and internal cluster IP is assigned to the service.
This means that it can only be reachable within the cluster. This is the default type when creating a service.


### NodePort for a Service

https://github.com/zealvora/certified-kubernetes-administrator/blob/master/Domain%203%20-%20Services%20and%20Networking/nodeport.md

NodePort exposes the Service on each Node's IP at a static port.

So you will be able to contact the NodePort service from outside the cluster by requesting to: `{IP}:{NodePort}`.

If a service type is NodePort then K8 will allocate a port on every worker node.


## Using Selectors in a Service

Currenlty we are manually defining the IP address of the PODS in Endpoints.

If there are 500 pods this is not managageable. 

So below is an example of creating a deployment with a service to then manage scaling and assignment.
  
##### Step 1: Creating Deployments
```sh
nano demo-deployment.yaml
```
```sh
apiVersion: apps/v1
kind: Deployment
metadata:
  name: nginx-deployment
  labels:
    app: nginx
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
        image: nginx:1.14.2
        ports:
        - containerPort: 80
```
```sh
kubectl apply -f demo-deployment.yaml
```

##### Step 2: Creating Service
```sh
nano service-selector.yaml
```
```sh
apiVersion: v1
kind: Service
metadata:
   name: kplabs-service-selector
spec:
   selector:
     app: nginx
   ports:
   - port: 80
     targetPort: 80
```
```sh
kubectl apply -f service-selector.yaml
```

##### Step 3: Verify Endpoints in Service
```sh
kubectl describe service kplabs-service-selector
```

##### Step 4: Scale Deployments
```sh
kubectl scale deployment/nginx-deployment --replicas=10
```

##### Step 5: Verify Endpoints in Service
```sh
kubectl describe service kplabs-service-selector
```

##### Step 6: Create a New Manual POD and Add a Label
```sh
kubectl run manual-pod --image=nginx
kubectl label pods manual-pod app=nginx
```

##### Step 7: Verify Endpoints in Service
```sh
kubectl describe service kplabs-service-selector
kubectl describe endpoints kplabs-service-selector
```

##### Step 8: Delete Created Resources
```sh
kubectl delete service kplabs-service-selector
kubectl delete -f demo-deployment.yaml
kubectl delete pod manual-pod
```


