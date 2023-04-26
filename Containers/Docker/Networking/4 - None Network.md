This is used to completely disable the networking stack on a container. 

If you look at `docker network ls` you can see the driver is set to null. As such it will not configure any networking or IP for that container. As such no one can connect and the container cannot connect outside at all.