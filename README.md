# docker-cheatsheet

### Dockerfile

- create an image from Dockerfile
```
docker build -t <image_name> <Dockerfile dir>
```

### General

- list images
```
docker images
```

- list containers
```
docker ps
```

- remove containers
```
docker rm -v (docker ps -a -q -f status=exited)
docker rm $(docker ps -a -q)
```

### Run

- running container with the image
```
docker run -p 80:80 <image_name>
```
- attach bash
```
docker exec -i -t <container_id> /bin/bash
```
- mount folder
```
docker run -v <host_dir>:<container_dir>
```
