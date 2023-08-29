Host network remove the isolation between the docker host and the containers to use the hosts networking directly.

For example if you run a container which bind port 80 and you use host networking, the containers application will be available on port 80 on the hosts IP address.

This differs from the bridge network that each has its own IP and would have to communicate to the bridge Gateway in order to talk out of itself.

To create a container that uses the host network you can reference [[2 - User Defined Networks#Assign a container to a network]]
