# MANAGING

## Basics

### Containers

#### List containers

```sh
docker container ps        # List only running containers
docker container ps -a     # List all containers
```

#### Start a container

```sh
docker container start <container_id>
```

#### Stop a container

```sh
docker container stop <container_id>
```

#### Remove a container

```sh
docker container rm <container_id>
```

#### Attach to a running container

```sh
docker attach <container_id>
```

#### Run a container interactively

```sh
docker run -it <image_name> /bin/bash
```

- `-i` keeps STDIN open.
- `-t` allocates a pseudo-TTY.

#### Name a container

```sh
docker run --name <container_name> <image_name>
```

#### Auto-remove a container after exit

```sh
docker run --rm <image_name>
```

#### Combine options

```sh
docker run -it --rm --name mycontainer <image_name> /bin/bash
```

- Starts an interactive shell, names the container, and removes it when done.

---

### Images

#### List images

```sh
docker image ls
```

#### Pull an image

```sh
docker image pull <image_name>
```

#### Remove an image

```sh
docker image rm <image_id>
```

---

### Volumes

#### List volumes

```sh
docker volume ls
```

#### Create a volume

```sh
docker volume create <volume_name>
```

#### Remove a volume

```sh
docker volume rm <volume_name>
```
