# docker-cli-commands
My quick reference for Docker CLI commands

## `docker build` vs. `docker create` vs. `docker start` vs. `docker run` vs. `docker-compose build` vs. `docker-compose run`

If you’re new to Docker, as I am, you may feel overwhelmed with the bewildering number of CLI commands that this product offers.

As I was just beginning, I was particularly confused with which CLI command to use to build/create, start, and run stuff in Docker because they seemed to have similar meanings or performed similar/overlapping actions.

What I found is that some commands perform just one type of action, while others combine multiple types of actions. This  provides the user the flexibility to perform tasks one at a time or all in one go. It depends entirely on each user’s strategy in creating containers/services.

As a reference for myself myself and other Docker newbies, here’s a summary of Docker CLI commands that are used for  building, creating, starting, running images/containers/services.

Please take note that the:
- `docker` base command is used for single containers
- `docker-compose` base command is used for multi-container applications

### `docker build`

Builds an image from a Dockerfile.

https://docs.docker.com/compose/reference/build/

### `docker create`

Creates (but not starts) a container from an image built from a Dockerfile.

https://docs.docker.com/engine/reference/commandline/create/

### `docker start`

Starts a container that has been previously created from an image built from a Dockerfile.

https://docs.docker.com/engine/reference/commandline/start/

### `docker run`

Runs a command on a container, but only after it performs the following actions behind the scenes:
- Creating a writeable container layer over the specified image
- Starting the container.

https://docs.docker.com/engine/reference/commandline/run/

### `docker-compose build`

Builds, rebuilds, and tags services. A rebuild needs to be done after a change to the service’s Dockerfile or the contents of its build directory.

https://docs.docker.com/compose/reference/build/

### `docker-compose create`

This command is deprecated. Use the `up` command with `—no-start` instead.

https://docs.docker.com/compose/reference/create/

### `docker-compose start`

Starts existing containers for a service.

https://docs.docker.com/compose/reference/start/

### `docker-compose run`

Runs a one-time command against a service.

https://docs.docker.com/compose/reference/run/

### `docker-compose up`

Builds, (re)creates, starts, and attaches to containers for a service. Unless they are already running, this command also starts any linked services.

https://docs.docker.com/compose/reference/up/
