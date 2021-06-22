# Useful docker commands

## Building docker images
* `docker build -t [tag-name] [dir-with-Dockerfile]`

## Run a docker image
* `docker run -dp [Your-port]:[exposed-docker-port] [image-tag]`
    * In background with port forwarding
* `docker run --net=host [image-tag]`
    * Run as localhost, useful for connecting to other containers
* `docker run --name=[your-name] [image-tag]`
    * Giving a custom name to the container, makes it easier to stop/restart
* `docker run -it [image-tag]`
    * runs the image in your terminal, useful to see the output
* `docker run -it [image-tag] bash`
    * runs a terminal inside your docker image

## Working with containers
* `docker ps`
    * Lists all running containers w/ ports
* `docker container ls -a`
    * Lists all containers, including stopped ones
* `docker stop [container-name]`
    * stops the container with that name
* `docker restart [container-name]`
    * restarts container name
* `docker rm [container-name]`
    * removes the container with given name (only one of each name allowed)
* `docker container prune`
    * removes all stopped containers
* `docker exec [container-name] bash`
    * runs a bash terminal inside a running container

## List images in registry
* `docker image ls`
    * list all images in registry
* `docker image tag [old-tage] [new-tag]`
    * copies an image and renames it to new-tag
