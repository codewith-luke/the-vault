This is a stateless server side application that stores and lets you distribute docker images.

Docker Hub is the most simple example of a docker registry.

An example of a way to push images to a registry is: https://hub.docker.com/_/registry

The above would be publishing to your own hosted registry but the below pattern remains the same for most registries.

But there are a consistent amout of steps to push to a registry.

```sh
docker tag {image}:latest {registry_rul}/{image}
```
This will create an image with the new name.

You will then have to push that to the registry:

```sh
docker push {new_image}
```

### Searching Registries

https://docs.docker.com/engine/reference/commandline/search/

To find an image in the registry:

```sh
docker seach {key}
```

You can then use filters to narrrow down your seach such as `--limit 5`

### Mobing Images Across Hosts

First we can save one or more images into a zip that we will then be able to send or load up on another host.

```sh
docker save {image} > {image}.tar 
```

To load up the images from a saved zip you would run the following:

```sh
docker load < {image}.tar
```