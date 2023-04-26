## Docker Images vs Containers

For full CLI docs:
https://docs.docker.com/engine/reference/commandline/cli/

We want to focus on: https://docs.docker.com/engine/reference/commandline/container/
when working with containers. As it is the new structuyre docker is moving and pushing towards.

### Image

This is a file which contains the dependencies and configurations to run an application.

To find existing images you can visit: https://hub.docker.com/

To pull down an image:

```shell
docker pull {image}
```

To confirm available images:

```shell
docker images
```

### Container

##### Running a container
This is basically the running instance of an image.

To run a docker container with an image:

```shell
docker container run --name {container_name} -dt -p 80:80 {image_id_or_name}
```

To delte a container when it stops running use the flag `--rm`.

**NOTE -** By passing *`-dt`*  you would be running the docker container in detached mode.

##### Port breakdown
By default your containers are not open for the outside world to look into. To do so you have to specify the port you want to expose external. So doing `8000:80` the **LHS (8000)** will be the **host** request will send to the **RHS (80)** which is a container.

To see a docker containers internal IP you can use

```shell
docker container inspect {image_name}
```

This will then show you a lot of details but at the bottom you can see:
![[Pasted image 20221019165145.png]]

You cannot connect to this private network from outisde of your container.

##### Container Status and Commands

To see currently running containers: 

```shell
docker ps
```

To then stop a docker container:

```shell
docker container stop {docker_image_name_or_id}
```

This is if you want to see all docker containers regardless if they are running.

```shell
docker ps -a
```

This means you are then able to get the name and then restart your container with:

```shell
docker container start {name}
```

If you are unsure the public IP you can run:

```shell
ifconfig
```

Once your container is running again you are able to also use `netstat -ntlp` to verify that your docker container is running on the specified port:
![[Pasted image 20221019162008.png]]
As well as running a `curl {ip}` to verify the http response and that it is running as expected.

#### Running  sub docker commands

When running a docker command like `docker stop {container}` you have to manually pass in each container if you had mutliple.

However there is a way that you can append extra information to build up more complex docker CLI commands. For example, lets combine the stop above with `docker container ls -aq` which would list all our containers ID's:

```shell
docker container stop $(docker container ls -aq)
```

This would now first go and get all our docker container ID's and then run them against docker stop. Essentially stopping all containers in a single command.

#### Remove a Container

To remove an unused container

```shell
docker container rm ${container_id_or_name}
```

You can optionally pass the `-f` to force close it. However it is recommended to first stop the container.
