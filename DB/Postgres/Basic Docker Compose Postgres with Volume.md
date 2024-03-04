Make sure to checkout [[1 - Docker Compose]] to understand how this works.

```yaml
version: '3'
services:
  disclone:
    env_file:
        - .development.env
    image: postgres
    volumes:
      - postgres-data:/var/lib/postgresql/data
volumes:
  postgres-data:
```