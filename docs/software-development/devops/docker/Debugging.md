# Debugging Docker Containers

See the logs of the container, or get into a terminal of the container to debug

- `docker logs <id>` or `docker logs <name>` to check the logs
- `docker exec -it <id> /bin/bash` to open an _interactive terminal_ (bash) inside the container. The cursor will change in the temrinal, indicating you are now inside the container terminal. Type `exit` to exit.

> [!TIP]
>
> - Can also use `docker exec -it <name> /bin/bash`
> - While in the terminal, type `env` to check the environmental variables

> [!WARNING]
> Since Docker images are usually built on top of very lightweight Linus distros, you won't have much commands like `curl` etc., but the basic ones should be enough for debugging
