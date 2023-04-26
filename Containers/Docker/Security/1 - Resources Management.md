## CGroups

cgroups (control groups) is a Linux kernel feature that allows administrators to limit, prioritize, and isolate the resources used by groups of processes. cgroups provides a hierarchical structure for organizing processes, and allows administrators to specify limits and constraints on the resources that can be used by each group. This can help to ensure that critical system processes have sufficient resources, and that individual users or applications do not consume too many resources. cgroups also allows administrators to monitor the usage of resources by each group, and provides mechanisms for controlling the allocation of resources in real-time. This can be useful for optimizing the performance of the system and ensuring that it remains stable and responsive.

## Commands

When connecting to a docker container you can use `free -m` to then see the amount of free memory. You can also use `top` to see processes and their memory usage. However these tools are not really considered 'cgroup aware'.

So using a command like:

```sh
cat /sys/fs/cgroup/memory
```

You can get a better idea of mem usage and so should be used over the others.

To see available options for memory management use `docker container --help` then scroll down till you see `-m`.


### Example: Restricting CPU

This is using the `--cpu` flag that will guarentee at most x amount of CPU.

```sh
docker container run -dt --name {name} --cpus=1.5 {image} sh
```

If you were to use something like `--cpuset-cpus`, you would the be able to limit the specific CPUs or cores a container can use. In this case it is comma seperated and specifies which CPU.

```sh
docker container run -dt --name {name} --cpuset-cpus=0,1 {image} sh
```

## Reservation VS Limits

By defualt a container has no resource constraint. It is thus important to ensure that it does not consume too much memory or CPU. Otherwise this can cause 'OM' or Out of Memory exceptions and start to kill high usage processes.

### Limit

This imposes an upper limit (ceiling) that can be used by a container.

### Reservation

This is less reigid than a limit. When the system is running low on memory and there is  contention, reservation tries to bring the container's memeory consumption at or below the reservation limit.



