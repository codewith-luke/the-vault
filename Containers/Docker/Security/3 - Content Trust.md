Docker content trust is a security feature of Docker that allows users to verify the integrity and publisher of Docker images. With content trust enabled, users can be sure that the images they are using are exactly what the publisher intended, and that they haven't been tampered with in any way. This can help to prevent malicious attacks and ensure that users are running the correct versions of images in their environments. To use content trust, users must have a set of cryptographic keys and must opt in to using content trust when they pull or push images to and from a registry.

To enable content trust you will run the following:

```sh
export DOCKER_CONTENT_TRUST=1
```
