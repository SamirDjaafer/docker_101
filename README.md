# Docker Cheat Sheet 

### Download Docker Desktop from Docker Hub

- Follow the installation guide
- Check docker is installed with `docker --version`

### Creating containers commands 

- `docker ps` - shows all running containers
- `docker ps -a` - shows all containers (even ones not running)
- `docker run {image}` - boot up a new container
- `docker run --name {name} {image}` - boot up a new container with a name
- `docker run -d {image}` - `-d` is used for detached mode
- `docker run -p 80:80` or `docker run -p 3000:80` - map ports 

Example of full command to boot up container

- `docker run --name website -d -p 3000:80 -p 80:80 -p 8080:80 nginx:latest`
