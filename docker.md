### Image Management
```bash
docker pull <image>:<tag>
docker images
docker rmi <image_name>
docker build -t <image_name:tag> .
docker push <username>/<repository>:<tag>
```

### Container Lifecycle
```bash
docker run <image>:<tag>
docker run -d <image>:<tag>
docker run -d -p <host_port>:<container_port> <image>:<tag>
docker run --name <container_name> -d -p <host_port>:<container_port> <image>:<tag>
docker ps
docker ps -a
docker stop <container_name_or_id>
docker start <container_name_or_id>
docker rm <container_name_or_id>
docker rm -f <container_name_or_id>
```

### Container Interaction
```bash
docker logs <container_name_or_id>
docker exec -it <container_name_or_id> <command>
docker inspect <container_name_or_id>
```

### Networking
```bash
docker network ls
docker network create <network_name>
docker network connect <network_name> <container_name_or_id>
docker network disconnect <network_name> <container_name_or_id>
```

### Volumes
```bash
docker volume create <volume_name>
docker run -v <volume_name>:<container_path> <image>
docker volume ls
docker volume rm <volume_name>
```

### Docker Compose
```bash
docker-compose up -d
docker-compose down
docker-compose ps
docker-compose logs
```

### System Maintenance
```bash
docker system prune
docker system df
docker info
```

### Notes:
- When using `docker run`, it will pull the image if it doesn't exist locally.
- The `-d` or `--detach` flag detaches the container, running it in the background.
    - NOTE: A running process will be required on the machine so docker keeps the process alive. For example: `docker run -d <image> tail -f /dev/null`.  In most real-world scenarios, the container would run an actual application or service.
- Port mapping is done with `-p host_port:container_port`.
- Use `--name` to specify a custom name for a container.
- The `-f` flag with `docker rm` forces removal of a running container.
- Use `docker exec` to run commands in a running container.
- `docker-compose` is used for managing multi-container applications.
- `docker system prune` removes unused Docker objects to free up space.
