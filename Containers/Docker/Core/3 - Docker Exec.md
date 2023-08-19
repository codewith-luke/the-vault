Docker container exec commands run a new command in a running container.

This means that if you have a container that is active you can execute commands inside of that container.

For example:

```shell
docker container exec -it {container_name} bash
```

Will allow you to run any binary that is within your container. So above we are execiting bash. Which then means we are able to run and see our NGINX status.

```shell
/etc/init.d/nginx status
```

To then exit your container either `ctrl + d` or type `exit`.

### Linux Process and  -it flag

Every process that we create in a Linux environment has 3 open file descriptors:

-  stdin (what you type in)
-  stdout + stderr (shows up on your screen)

When using flags for exec as above we use `-it` 

`-i` flag will mean that we keep the stdin open when executing our command
then when adding the `-it` this gives you a *tty*. So if you had to run this without the `i` and just the `t` you would then not be able to pass in a (**stdin**). 

By combining these two flags you then are able to use the stdin and have a tty. Creating an interactive terminal within your container.

