# Docker Deployment

## Checkpoint 3 - Docker Environment

### Check Docker Version

```bash
docker --version
```
### Check Docker Information
This command displays the installed Docker version.
```bash
docker info
```
This command displays information about the Docker client and server environment.

## Checkpoint 4 - Deploy Your First Container
```bash
docker pull nginx 
This command downloads the official Nginx image from Docker Hub.

docker run -d -p 8080:80 --name nginx-server nginx 
This command runs the Nginx container in detached mode and maps port 8080 on the host to port 80 inside the container.

curl http://localhost:8080 
This command sends an HTTP request to the Nginx web server and verifies that it is running successfully. The command successfully displayed the Nginx welcome page containing "Welcome to nginx!".

Checkpoint 5

docker ps 
This command lists the currently running Docker containers.

docker stop nginx-server 
This command stops the running Nginx container.

docker ps 
This command verifies that the Nginx container is no longer running.

docker rm nginx-server 
This command removes the stopped Nginx container.

docker ps 
This command verifies that there are no running containers after the Nginx container was removed.


