# Docker Deployment

## Checkpoint 3 - Docker Environment

### Check Docker Version

```bash
docker --version
```
This command displays the installed Docker version.
### Check Docker Information
```bash
docker info
```
This command displays information about the Docker client and server environment.

## Checkpoint 4 - Deploy Your First Container

### Pull the Nginx Image
```bash
docker pull nginx
```
This command downloads the official Nginx image from Docker Hub.

### Run the Nginx Container
```
docker run -d -p 8080:80 --name nginx-server nginx
```
This command runs the Nginx container in detached mode and maps port 8080 on the host to port 80 inside the container.

### Test the Nginx Web Server
```
curl http://localhost:8080
```
This command sends an HTTP request to the Nginx web server and verifies that it is running successfully. The command successfully displayed the Nginx welcome page containing "Welcome to nginx!".

## Checkpoint 5 - The Container Lifecycle

### The Container Lifecycle
```
docker ps
```
This command lists the currently running Docker containers.

### Stop the Container
```
docker stop nginx-server
```
This command stops the running Nginx container.

### Verify the Container Is Stopped
```
docker ps
```
This command verifies that the Nginx container is no longer running.

### Remove the Container
```
docker rm nginx-server
```
This command removes the stopped Nginx container.

### Verify the Container Removal
```
docker ps
```
This command verifies that there are no running containers after the Nginx container was removed.


