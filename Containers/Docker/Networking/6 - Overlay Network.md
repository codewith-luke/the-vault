The overlay network adriver creates a distributed network among multiple docker daemon hosts.

Overlay network allows containers connected to it to communicate securely.

So for example if you have a swarm cluster with 3 nodes. Each node is running a webserver. These webservers would not be able to communicate to each other over something like a bridge network. You would have to use an overlay network.

This network become automatically available after creating a swarm.

## Secure Overlay Network

In an overlay network the container can be spread acorss multiple servers. It is thus recommended to secure this communication. This is done using the encrypted flag.

```sh
docker network create --opt encrypted --driver overlay {name}
```

This ceates an *IPSEC* tunnel between all nodes where tasks are scheduled for servcies attached in the overlay network.

These tunnels use the *AES* algorithm in *GCM* mode. Manager notes automatically rotate the keys every 12h.

**Overlay encryption is not supported on windows. If a windows node attempts to connect to an encrypted overlay netowkr no error will show but it will not work.**
