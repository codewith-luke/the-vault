Nodes in a swarm use mutual TLS to authenticate, authorise and encrypt communications with other nodes in the swarm.

By default the manage node generates a new root Certificate Authority (CA) along with a key pair, which are used to secure communications with other nodes that join the swarm.

You can specify your own externally generated root CA, using the `--external-ca` flag on the docker swarm init command.

## Token Rotation and Nodes

When running `docker swarm ca --rotate` you will not have to update other worker nodes with new tokens. This is because the new root CA is signed by the previous. Once it has been rotated the old one will be removed from that node.

You would have to update the worker nodes token if that node left the swarm and a new root CA was assigned.


### Important Cert Notes

- Each node in a Swarm renews its certs every 3 months
- You can configure this interval using `docker swarm update --cert-expiry {time}`
- In event that a cluster CA key or manager node is compormised, you can rotate the swarm root CA so that none of th nodes trust certificates signed by the old root CA.

## Managing and Creating Secrets

To create an easy way to manage secrets you can create a secrets file and then use:

```sh
docker secret create {name} {file}
```

Then in order to use this when creating a service you would then use:

```sh
docker service create --name {service} --secret {secret_name} {image}
```

To then see secrets within a container first connect to your container then head to `cd /run/`. This is where all secrets are generally stored in a container.