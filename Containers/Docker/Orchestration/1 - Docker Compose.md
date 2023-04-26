Compose is a tool for defining and running multi-container docker applications.
This is all done via a YAML file.

If you are running Docker on Linux you will first need to install Docker compose:

https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-compose-on-ubuntu-20-04

## Creating a Config

Below is a config example for a basic docker-compose.yml file. The key parts to understand here is that we are creating 2 services and defining their images that they will be using.

```yaml
version: '3'
services:
  webserver:
    image: nginx
    ports: 
	    - "8080:80"
  database:
    image: redis
```

To the validate a config use `docker-compose config`

#### Start Docker Compose

```sh
docker-compose up -d
```

#### Stop Docker Compose

```sh
docker-compose down
```