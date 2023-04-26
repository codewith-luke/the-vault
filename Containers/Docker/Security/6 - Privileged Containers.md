By default docker containers do not have many capabilities. Docker containers cannot access the device they are on.

Privileged containers can access all the devices on the host as well as have configuration in AppArmor or SELinux to allow the container nearly all the same access to the host as processes running outside the container on the host.

- Limits that you set for privileged containers will not be followed
- Running a privileged flag gives all the capabilities to the container.

```sh
docker run -dt --privileged {image} {cmd}
```