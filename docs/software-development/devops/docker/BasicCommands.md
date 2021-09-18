# Docker Basic Commands

- `docker pull`
  Pulls an image to local machine
- `docker start`
  Starts a container. Note: With `start`, you are working with a container and not image
- `docker run`
  Pulls an image if not locally available and starts a new container. Flags:

  - `docker run -d` or `docker run --detach`
    Run in detached mode so you can still use terminal
  - `docker run -p` to bind port of your host/local machine to the port of the container like `docker run -p3000:6974 redis`.
    6974 is the port of the container and 3000 of your local machine
  - `docker run -d --name redis-older redis:4.0` to overirde the default name

- `docker stop`
  Stops a running container. Will retain configuration like custom name or port binding.

> [!TIP]
> Restart a container by `docker stop` then `docker start` to reflect some new changes

- `docker ps`
  Show running containers

- `docker ps -a`
  Show all containers

- `docker images`
  Show all images you have locally, can be used to discard stale images and clear storage space
