To see a list of capabilities you can add and what are assigned by default:
https://docs.docker.com/engine/reference/run/

When creating your container you can then add and remove these as per the following:

```sh
docker run -dt --name {name} --cap-add {cap} {image}
```