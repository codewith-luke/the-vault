Volumes are great for persisting data. Docker has 2 options for this: volumes and bind mounts. On Linux you also have access to tmpfs mount.


### Create and using a Volume

```sh
docker volume create {name}
```

```sh
docker container run -dt --name {name} -v {volume}:{dir} {image} sh
```

Volumes can then be found:

```cd
cd /var/lib/docker/volumes
```

## Creating a Bind Mount

With a bind mount you use a file or directory on the host machine and it is mounted into a container, these need to be made Readonly if you dont want to be able to change it directly in the container. There are 2 ways to do this:

```sh
docker container run -dt --name {name} -v {path}:{out_path} {image} sh
```

```sh
docker container run -dt --name {name} --mount=bind,source={path},target={path} {image} sh
```