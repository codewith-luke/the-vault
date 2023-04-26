# Table of Content

[[1 - Bridge Networks]]
[[2 - User Defined Networks]]
[[3 - Host Network]]
[[4 - None Network]]
[[5 - Port Publishing]]
[[6 - Overlay Network]]

Within a docker container you have access to a few different network drivers.

Docker takes care of networking aspects so that containers can communicate with each other as well as the docker host.

There are several drivers available:

- bridge
- host 
- overlay
- macvlan
- none

To view all available networks you can use `docker network ls`. This will allow you to see networks and drivers on that instance. You can then get more information on a driver by using `docker inspect {driver_name}`.

To inspect the containers in a network you would use `docker network inspect {network}`.
To then see what driver a container is running use `docker container inspect {container}`.