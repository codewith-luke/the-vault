This document will go over more complicated commands, however a full list of commands for docker images can be found: https://docs.docker.com/engine/reference/commandline/image/
Or `docker image --help`

### Image Tagging

When building you may want to tag your image. This can be done with the `-t` flag.

`docker build -t {image_name}:{tag} .`

You can also tag an image that is already build with the tag command.

`docker tag {image_id} {image_name}:{tag}`

The above will not only name your image. But will also give it a tag.

To tag an existing image with a previous tag and create a new one:

`docker tag {image_id}:{tag} {image_name}:{new_tag}`

This will not remove the original but create a new one with same image ID

### Docker Inspect

To inspect an image and its details:

```sh
docker image inspect {image_name}
```

You can use linux grep top then find specific details

```sh
docker image inspect {image_name} | grep hostname
```

Or the preffered is using the format flag

```sh
docker image inspect {image_name} --format='{{.Id}}'
docker image inspect {image_name} --format='{{json .ContainerConfig}}'
docker image inspect {image_name} --format='{{.ContainerConfig.Hostname}}'
```

### Pruning

This helps us cleanup unused images (only dangling images - Image with no tages and not referenced by any container).

```sh
docker image prune
```

You can also use the `-a` flag will then remove any image with no container assocaited to it.

**Important to know pruning applies to images/containers/networks**