Docker storage drivers are responsible for managing the data used by Docker containers. The storage driver determines how the Docker engine stores and manages the data for containers. Some common storage drivers include `aufs`, `devicemapper`, `overlay`, and `zfs`. Different storage drivers have different capabilities and can be better suited for different use cases. For example, some storage drivers are more efficient at handling large numbers of small files, while others are better at handling a smaller number of large files. It's important to choose the right storage driver for your application to ensure optimal performance and reliability.

To see the storage type use:

```sh
docker info
```

You can also view the storage in:

```sh
/var/lib/docker
```


## Copy on Write

CoW, or "Copy-on-Write", is a technique used by Docker storage drivers to improve the performance and efficiency of managing data for containers. The basic idea behind CoW is that, instead of copying the entire data set for a container each time a change is made, the storage driver only copies the specific data that has been modified. This can save significant amounts of time and resources, particularly when dealing with large data sets or multiple containers that share a common data set.

## Changing Driver

**NOTE: Changing your storage driver will result in you not being able to access previous version of storage or their containers.**

```sh
systemctl stop docker
```

```sh
cd /etc/docker
```

```sh
vim daemon.json
```

```json
{
	"storage-driver": "overlay2"
}
```

```sh
systemctl start docker
```
