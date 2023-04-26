## What is it?
The bridge network uses a software bridge which allows container connected to the same bridge network to communicate, while providing isolation from containers which are not connected to that bridge network.

**By default when creating a container it will get created in the bridge network.**

#### Example
If we inspect the docker bridge driver we can see some config information. If we pay attention to the Gateway this is the entry gateway that would have to be communicated to in order to talk out to the internet.

![[Pasted image 20221121163738.png]]

Then if we look at if we had running containers we can see that the IPv4 address falls under the subnet that was originally listed in the config. This container would need to talk to the Gateway IP to communicate out thereafter.

![[Pasted image 20221121163851.png]]

The important takeaway here is that a bridge network basically segments your containers and allows them to communicate to one another and have to talk to the Gateway to communicate outwards.