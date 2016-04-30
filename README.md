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

### Run

- running container with the image
```
docker run -p 80:80 <image_name>
```
- attach bash
```
docker exec -i -t <container_id> /bin/bash
```

- 
