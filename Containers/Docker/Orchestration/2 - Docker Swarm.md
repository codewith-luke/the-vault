https://www.interviewcake.com/concept/java/lru-cacheWhen refferring to a node we are reffering to an instance of the Docker engine participating in the swarm. To deploy your application to a swarm you would submit a service definition to a manger node.

## Creating Manager Node and adding Workers

The manager node is any one of the nodes (VMs) that you decide. The manager node dispatches units of work called tasks to worker nodes.

```sh
docker swarm init --advertise-addr {manager_ip})
```

Once this is run it will give you back a command something to the key of:

```sh
 docker swarm join --token {token}
```

![[Pasted image 20221122165448.png]]
When your workers have joined the swarm you should see something along these lines.

To add other managers to a swarm:

```sh
docker swarm join-token manager
```

This will give you the step to then join as a manger node. Similar to `swarm join` above.

See [[#Split Brain Problem and Quorum]] when creating and setting up workers and managers.

### Manager Only Node

Manager nodes by default also act as workers. This is not recommended as they have a lot of responsobility [[#High Availability of Swam Manager Nodes]]

To ensure that the node only acts as a manager node you would need to drain the leader node [[#Draining Swarm Node]]

## Services, Tasks and Containers

To see all current services use `service ls`.

A service is the definition of the tasks to execute on the manager or worker nodes.

```sh
docker service create --name webserver --replicas 1 nginx
```

With the above script we are creating a service called `webserver` this will start up a task per replica (**Containers in a service are called tasks**). using the nginx image.

Once create your can then use `docker service ps {service_name}` to then see your service and get more details on what and where it is running.

If you have run the above and then ran `docker ps` you will be able to see your container running. If you had to stop that container then run `docker service ps {service_name}` again you can then see that it has started up a new nginx container.

This is because our service will ensure that we always have 1 nginx replica always running as we specified. It will decide which swarm node it will run on. It may not always be the same node.

#### Remove service

To remove a serivice use:
```sh
docker service rm {service_name}
```

When doing this it will also shut down all running contianers on the relevant nodes.

## Scaling Service in Swarm

Once you have deployed a service to a sawrm you can use the Docker CLI to scale the number of containers.

So if you have create your service as per above you may want to scale your service up or down.

There are two approaches and both be used to then create more tasks based on the service replica originally set. This is both for upscaling and dowscaling.

##### Approach 1

```sh
docker service scale {service_name}={amount}
```

##### Approach 2

```sh
docker service update --replicas {amount} {service_name}
```

The difference between the 2 approaches is with the first command we can actually specify multiple services at the same time. Where as approach 2 can only do a specific service.

## Replicated vs Global Service

A replicated service, you specify the number of identical tasks you want to run. For example if you want to deploy and nginx service with 2 replicas each serving same content.

**Example**

```sh
docker service create --name replicaservice --replicas 1 nginx
```

A global service is a service that runs one task on every node. Each time you add a node to the swarm, the orchestrator creates a task and the scheduler assings the task to the new node.

**Example**

```sh
docker service create --name globalservice --mode global -dt ubuntu
```

Now the the key difference here is we are passing a mode and specifying global and in doing so we are telling this to run this service across all of the nodes in that swarm. You can confirm this by running `docker service ps globalservice`.

## Draining Swarm Node

A good use case for this is you may have a monthly life cycle and want to update one of the nodesin a swarm or some form of maintenence. 

To take a node out you need drain it so that the tasks are distributed to the other nodes.

```sh
docker node update --availability drain {node}
```

Run `docker node ls` to see the availability.

So if we now had to scale this service since the node has been flagged as drained it will not add new tasks to that specific node.

To make this no longer the case we need to mark the node as active.

```sh
docker node update --availability active {node}
```

This will not re-distribute tasks to the now active node.

## Inspecting Swarm Services and Nodes

In order to get detailed information about a service:

```sh
docker service inspect {service_name}
```

You can then use the `--pretty` flag to make it more readable.

You can then inspect and find out information about a node in a swarm as well.

```sh
docker node inspect {node} --pretty
```

## Adding Network and Publishing Ports to Swarm Tasks

If for example you run the following

```sh
docker service create --name myweb --replicas 2 nginx
```

This will not publish the ports for that nginx webserver on those nodes.

In order to do this create your new service but we will specify the port mappings:

```sh
docker service create --name myweb --replicas 2 --publish 8080:80 nginx
```

## Swarm with Docker Compose

*First make sure you understand [[1 - Docker Compose]].*

In previous examples we created services across our swarm nodes. Now if we are wanting to do the same but using multiple services we have to make use of a compose file and then use `docker stack`

Using the example docker compose in the above link we can start a distributed stack across our nodes using the following:

```sh
docker stack deploy --compose-file docker-compose.yml {stack_name}
```

The interesting thing to note is when looking at `docker stack ps {stack_name}`. It will tell us where these services are running in our swarm.

To then remove your stack run `docker stack rm {stack_name}`.

## Locking a Swarm Cluster

Swarm clusters can contain a lot of sensitive data such as:

- TLS keys
- Encrypt and Decrypt keys

To automatically lock a swarm when it is resarted run:

```sh
docker swarm update --autolock=true
```

This will generate a key that you will need to save somewhere safe as whenver you try to unlock your swarm it will prompt you for it.

**To unlock:**
```sh
docker swarm unlock
```

**Retrieve Key:**
Once you have already unlocked the swarm you can retreive the key again using
```sh
docker swarm unlock-key
```

**Rotate Key:**
```sh
docker swarm unlock-key rotate
```

## Troubleshooting Swarm Service Deployment

There may be instances where a service is configured that no node in the the swarm can run its tasks. This puts the service into a *pending* state.

Some examples:

- All nodes are draned, you create a service, it is pending until a node becomes available
- You can reserve a specific amount of memory for a service. If no node in the swarm has that amount of memory the service will remain in pending.
- You imposed some kind of placement contraints.

To start you can first use `docker service ps {service_name}` to see the state of services. Find the one that is stuck in pending.

You can then go ahead and do a `docker inspect {id}` if the stuck task. Scroll down to status and you can get some information as to the reason.

## Mounting Volumes via Swarm

To create a service with a volume:

```sh
docker service create --name {service_name} --mount type=volume,source={volume_name},target=/{path} nginx
```

Then verify where the host of the created service: 

```sh
docker service ps {service_name}
```

Verify the volume information:

```sh
docker volume ls
```

**If you remove a service that you created a volume for it will keep that volume and it's data**

## Control Service Placement

Sometimes you may want to create contstraints for which control scale and placement of services on different nodes.

You can create constraints using things such as:
- Placement contstraints such as using labels
- Resource constraints such as CPU and memory requirements
- Placement Preferences

To specify a constraint you would write something such as:

```sh
docker service create --name {service_name} --contraint node.labels.region=={region} --replicas 3 {image_name}
```

### Add a label to a node

When building contraints you may want to add a label or update your node to meet these constraints:

```sh
docker node update --label-add region={region} {node_id}
```

## Creating Services using Templates

We can make use of templates whe creating services.

```sh
docker service create --name {name} --hostname="{{.Node.Hostname}}-{{.Service.Name}}" nginx
```

The above data inside `{{}}` are templates that allow placeholders that would be populated with data. So above it would populate the first with the hostname of the server and then the service name. These are templates for creating and populating data. To see all place holders visit: https://docs.docker.com/engine/swarm/services/

You can also only use templates for `--hostname`, `--mount`, `--env`.

## Split Brain Problem and Quorum

Split brain problem refers to when you have two nodes running in a swarm. One has to be a master and others are slave nodes. If the slave cannot communicate, due to some connectivity issue, to the master node it would then upgrade itself to the master node. Which mean you could have 2 master nodes running at the same time. 

![[Pasted image 20221125172704.png]]

This is a problem if it was the resposobility of the first master node to read/write to some form of persistent storage. Now that you create two this can introduce problems.

![[Pasted image 20221125172652.png]]

### Introducing Quorum

Quorum as a concept is about having 3 nodes within a cluster. Each node in a cluster has a vote. This means the if the master node has communication issues like previously that in this example here we can see a LHS and a RHS. The RHS is made of 2 nodes which means they have a combined vote power of 2. Meaning they would win.

![[Pasted image 20221125173042.png]]

As a result it would then disconnect the VM1 from the central storage and designate one of the other nodes to become the new master.

![[Pasted image 20221125173143.png]]

This means when node 1 is restored it will then become a passive node.

![[Pasted image 20221125173252.png]]

In the above example if we have 3 nodes it means we can only have a failure of 1. Another failure will bring us back to the original split brain problem. As you introduce more nodes you would increase the majority and the fault tolerance.

![[Pasted image 20221125173520.png]]

With the above you can see that having an even amount of nodes does not increase the fault tolerance. **So it should maintain an odd number of nodes.** This is know as a **Quorum**.

	An N manager cluster tolerates the loss of at most (N-1)/2 managers.

### High Availability of Swam Manager Nodes

Manager nodes have a lot of responsobility. So You want to ensure they are high availability.
These responsobilities include:

- maintaining cluster state
- scheduling services
- serving swarm mode HTTP API endpoints

Using a Raft implementation, the managers maintain a consistent internal state of the entire swarm and all services running on it.

### Recover from losing the Quorum

Based on the fault tolerance for you cluster ([[#Introducing Quorum]]) you may come into a situation where the cluster cannot fail again. 

1) Start the swarm again (not recommended)
2) Force new cluster

To force a new cluster you would do:

```sh
docker swarm init --force-new-cluster --advertise-addr {ip:port}
```

This will help recover your previous managers and get you back up and running.