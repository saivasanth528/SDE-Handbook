# Docker Basic Commands

- `docker pull`
  Pulls an image to local machine
- `docker start`
  Starts a container
- `docker run`
  Pulls an image if not locally available and starts the container. Flags:

  - `docker run -d` or `docker run --detach`
    Run in detached mode so you can still use terminal
  - `docker run -p` to bind port of your host/local machine to the port of the container like `docker run -p3000:6974 redis`.
    6974 is the port of the container and 3000 of your local machine

- `docker stop`
  Stops a running container

> [!TIP]
> Restart a container by `docker stop` then `docker start` to reflect some new changes

- `docker ps`
  Show running containers

- `docker ps -a`
  Show all containers

- `docker images`
  Show all images you have locally, can be used to discard stale images and clear storage space
