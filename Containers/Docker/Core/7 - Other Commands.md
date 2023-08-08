## Default Container Commands

The default container command is the *command* that gets executed when you run your container.

![[Pasted image 20221025125940.png]]
So when we have a running container the above circles command is what would have veen run to start that containers process. This typically runs as **PID 1**.

These commands can be found in the relevant docker file in that image.

### Change default container command

1)  Change the docker file in the image itself
2)  Run override on container run
   
```
docker container run -d {image_name} {command}
```

## Restart Policies

By default docker containers will not start when they *exit* or when the daemon is *restarted*.

Docker provides us with something called restart polocies. Basically we tell it when it should restart.
This is useful for when your server restarts and you need your dopcker container to restart.

There are four flags for policies:
https://docs.docker.com/config/containers/start-containers-automatically/

To run a new container with a policy use the above to configure it. If you need to change an existing containers polixy run the following:

```
docker update --restart {policy} {container}
```

## Disk Metrics

Similar to [[Useful Commands#Disk Usage]] we can also see the metrics for our docker container using `df`

```
docker system df
```

Will then give us metrics on our images and containers.

```
docker system df -v
```

Will then allow you to see the metrics per component and it will order it from highest to lowest.

## Automatic Container Deletion

Sometimes you may want to have a container exit automatically when it is done. This can be configured with the `--rm` flag.

```
docker container run -dt --rm --name {container_name} {image_name} {command}
```

When this completes it will the remove the container automatically for you.

## Docker Commit

When you make changes in a container it is useful to create a new image with these changes. 

```sh
docker container commit {container_id} {new_image_name}
```

So what this will essentially do is take your existing running container and create a snapshot of that as a new image.

This becomes useful as you can then modify things such as commands on env variables as an example:

```sh
docker container commit --change='CMD ["ash"]' {container}
```

### Rem/licenseove All Containers

To stop and remove all running containers:

```sh
docker ps -aq | xargs docker stop | xargs docker rm
```

## Docker System Commands

https://docs.docker.com/engine/reference/commandline/system/

### Docker System Events

This allows you to get server events.

https://docs.docker.com/engine/reference/commandline/system_events/

This is useful for automation of tasks when certain things occur.