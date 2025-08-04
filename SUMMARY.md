## Docker Basics Summary

Docker is a platform for developing, shipping, and running applications inside containers. Here are some fundamental concepts:

### What is a Docker Image?

A Docker image is a lightweight, standalone, and executable package that includes everything needed to run a piece of software: code, runtime, libraries, environment variables, and configuration files. Images are immutable and serve as the blueprint for containers.

### Running Containers from Images

To run an application, you create a container from an image. Containers are isolated environments where your application executes.

### Binding Ports

When running a container, you often need to access its services from your host machine. You can bind ports using the `-p` flag:

```bash
docker run -p <host_port>:<container_port> <image_name>
```

For example, to run an image named `nodeapp` and bind port 3000 on your host to port 80 in the container:

```bash
docker run -p 3000:80 nodeapp
```

### Images are Read-Only

Docker images are read-only. When a container runs, a writable layer is added on top of the image, allowing the container to make changes without affecting the original image.
