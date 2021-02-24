# Useful docker commands

## Build container from Dockerfile
```
docker builde -t [tag-name] [dir-with-Dockerfile]
```

## Run a docker image
In background with port forwarding
```
docker run -dp [Your-port]:[exposed-docker-port] [image-tag]
```

## List images running
```
docker ps
```

## Run interactive bash in docker
```
docker run -it [image-tag] bash
```