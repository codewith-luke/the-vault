By default docker will use a bridge network. However you may decide a user-bridge is better suited.

These provide better isolation and interoperability between containerized applications.

As well as:

- Automatic DNS between containers
- Attach and detach from user-defiend networks on the fly
- Each user-defined network creates a configurable bridge
- Linked containers on the default bridge network shares environment variables

https://docs.docker.com/network/bridge/

## Creating a User Defined Network

To create a new netowork you first run:

```sh
docker network create --driver {driver} {network_name}
```

If you do not specify a driver it will by default use bridge.

You can then see your new network with `docker network ls`.

To use your new network:

```sh
docker container run -dt --name {container_name} --network {network_name} {image}
```

Then using `docker inspect {network_name}` you can then see the details of your newly created network.

You will also then be able to see your new network when running `ifconfig` as well as the original default birdge `docker0`.

### Assign a container to a network

You will then want to add containers to your new network. To do this run:

```sh
docker container run -dt --name {container_name} --network {network_name} {image}
```

