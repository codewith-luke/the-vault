## Getting Started

1) First choose a server provider (Digital Ocean, Azure etc). Then go ahead and create a basic server running Ubuntu and configure any other settings.

2) Once asked about SSH we want to go ahead and create an SSH key

```shell
ssh-keygen
```

Run through the steps. This will create a private and public key. Upload the public key to your server (**NOTE**: some providers may need you to first connect to your instance via a password and then you create SSH and then remove password auth).

3) Now you can connect to your new instance

```shell
ssh -i {private_key} {root_ser}@{ip}
```

## Updating your new Instance and installing Docker

Simply follow the below for either updating or setting up your new docker instance: 

https://docs.docker.com/engine/install/ubuntu/

When done check docker is running with:

```shell
systemctl status docker
```

![[Pasted image 20221019125758.png]]

As well as you can see docker information with:

```shell
docker info
```

![[Pasted image 20221019125919.png]]