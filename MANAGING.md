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
