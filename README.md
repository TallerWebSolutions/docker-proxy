# Docker Proxy

Docker container using Nginx proxy for running multiple development servers on the same host machine.

# Starting

`make run`

# Adding new container

To add a new app container to the proxy, just run it setting the `VIRTUAL_HOST` environment variable. E.g.:

```
my-app:
  image: my-image
  container_name: my-app
  environment:
    - VIRTUAL_HOST=my-app.domain.com
```
