# Mission 4: The Cloud-Native Engineer

## Mission Overview

This laboratory activity focused on cloud-native technologies, particularly Docker containers. I learned the difference between Virtual Machines and containers and used the KillerCoda Playground to deploy an Nginx web server. I also practiced managing the lifecycle of a Docker container.

## Objectives

- Differentiate between Virtual Machines and Containers.
- Access a Docker-enabled cloud environment using KillerCoda.
- Execute fundamental Docker CLI commands.
- Pull and run an Nginx container.
- Map a host port to a container port.
- Manage and remove a Docker container.
- Document container operations using Markdown.

## Docker Commands Executed

### Check Docker Version

```bash
docker --version
```
### Check Docker Information
```
docker info
```

### Pull Nginx Image
```
docker pull nginx
```

### Run Nginx Container
```
docker run -d -p 8080:80 --name nginx-server nginx
```

### Test Nginx Web Server
```
curl http://localhost:8080
```

### List Running Containers
```
docker ps
```

### Stop Nginx Container
```
docker stop nginx-server
```

### Verify Container Status
```
docker ps
```

### Remove Nginx Container
```
docker rm nginx-server
```

### Verify Container Removal
```
docker ps
```

## Skills Learned

I learned how to verify a Docker installation, download a Docker image, create and run a container, map network ports, test a containerized web server, and manage the container lifecycle. I also learned how containers provide a lightweight and fast way to deploy applications.

## Challenges Encountered

One challenge I encountered was remembering the correct Docker command syntax. I initially typed docker pill nginx instead of docker pull nginx. I also initially used HTTPS when testing the Nginx server, but the correct HTTP command successfully displayed the Nginx welcome page. These errors helped me understand the importance of using the correct commands and port configuration.
