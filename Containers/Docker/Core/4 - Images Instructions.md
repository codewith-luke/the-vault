In order to create a custom image you first need to create a docker file with the instructions to do so.

A basic example of an NGINX docker file looks like:


```Dockerfile
# DockerFile
FROM ubuntu
RUN apt-get update
RUN apt-get -y install nginx
CMD ["nginx", "-g", "daemon off;"]
```

## Breaking Down Dockerfile

`FROM`  is the base image we want to use for our image. In the above case we would use Ubuntu

Thereafter are the commands that we want to execute in our Dockerfile.

### Build

Once you are happy with your Dockerfile you can then run

```shell
docker build -t {tag_name} {dockerfile_path}
```

This will then be added to your images once done.

You can then run your image in a container by using the image ID and running through [[1 - Basics#Container]]

### Copy vs Add Instruction

```docker
FROM busybox
COPY copy.txt /tmp
ADD add.txt /tmp
CMD ["sh"]
```

In the above example we are using the base image of busybox and then copying the contents using add and copy and putting them into a tmp folder.

These both serve a similar purpose. They allow you to copy files from a location.

**Copy** takes a source and a destination. So it only lets you coppy in a loca file or a directory from the host.

**Add** is the same but also supports 2 other sources:
- You can use a URL instead of a directory (this is advised against and it is better to use curl or wget via `RUN` command)

```docker
RUN mkdir -p /usr/src/things \
| tar =xJC /usr/src/things \
&& make -C  /usr/src/things all
```

- You can extract a tar file from the source into a destination

```docker
ADD compress.tar.gz /tmp
```

### Expose Instruction

This is to inform the docker container to listen on a specified port. It functions as a type of documentation for a person running the docker image.

```docker
docker run -d --name web -p 80:80 nginx
```

So in the above example we are creating a container from nginx and saying we want to allow the **host** port 80 to map to the **containers** port 80.

Using `EXPOSE 9080` within our image is not actually doing anything other than informing the person using the image that there will be something within this image running on port `9080`

### Healthcheck Instruction
https://docs.docker.com/engine/reference/builder/#healthcheck

To perform health checks and monitor our container we can add the instruction below to monitor and let us know the status of our container when run.

```
HEALTHCHECK --interval=5s CMD ping -c 1 {IP}
```

You can also use `docker container inspect {container}` to look at the healthcheck logs.

Arguments:
- `--interval=`
- `--timeout=`
- `--start=period=`
- `--retries=`

If you want to add health check as you are running a container you run:

```shell
docker run -dt --name {name} --health-cmd "curl -f http://localhost" {image_name} sh
```

The above will attempt to run a health check with the default config (which would timeout if there is nothing running). You can then pass these arguments above to overwrite the defaults.

### CMD instruction vs Entrypoint

In a dockerfile you can specify an entrypoint instruction:

```
ENTRYPOINT ["/bin/ping"]
```

Unlike the `CMD` instruction the `ENTRYPOINT` instruction cannot be fully overriden. Only built on or appeneded.

### Workdir Instruction

This is setting the working directory for any `RUN, CMD, ENTRYPOINT, COPY, ADD` instruction that follow it. Think of it as file hopping.

```sh
FROM busybox
RUN mkdir /root/demo
WORKDIR /root/demo
RUN touch file1.txt
CMD ["/bin/sh"]
```

The above will create a demo directory and then set the working directory for the docker container. Which means when we create a fil it will be created at that location.

You can then start to swap working directories but remember it will always be the last execution of `WORKDIR`

```sh
FROM busybox
RUN mkdir /root/demo/context1/context2
WORKDIR /root/demo
WORKDIR context1
WORKDIR context2
RUN touch file1.txt # is in context2
CMD ["/bin/sh"]
```

### ENV Instruction

This instruction allows you to create `key:value` pairs for a docker image.

```sh
FROM busybox
ENV NGINX 1.2
RUN touch web-$NGINX.txt
CMD ["/bin/sh"]
```

In the above case we have an env variable called `NGINX=1.2`

You can also use `-e`, `--env` or `--env-file` flags to set simple env variables for your container when running.

To see envionment variables when connected to a running container run `echo ${ENV_VARIABLE}`


