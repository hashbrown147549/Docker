# Docker
## Basic Commands
### To pull an Image
  docker pull IMAGE NAME
  Example: docker pull hello-world

### To pull a specified version of an image
  docker pull IMAGE_NAME:version(default latest)

### To know the images present in your docker desktop
  docker images

### To run a container in that Image
  docker run IMAGE_NAME
### To run a docker image in an interactive mode
  docker run -it IMAGE_NAME

### To get all containes
  docker ps -a

### To get running containers
  docker ps
###To start an  existing container
  docker start CONTAINER_ID/CONTAINER_NAME

###To stop a running container
  docker stop CONTAINER_ID/CONTAINER_NAME

#### Note: In order to delete a docker image you need to delete all the containers made on that image
### To delete a docker container
  docker rm CONTAINER_ID/CONTAINER_NAME

### To delete a docker image
  docker rmi IMAGE_ID/IMAGE_NAME

  docker run -d -e MYSQL_ROOT_PASSWORD=secret IMAGE_NAME
  docker run -d -e MYSQL_ROOT_PASSWORD=secret --name mysql_older IMAGE_NAME:version

### PORT BINDING
  docker run -pHOST_PORT:CONTAINER_PORT

### TROUBLESHOOT COMMANDS
1. docker logs CONTAINER_ID
#### accessing shell or bash of that container
      docker exec -it CONTAINER_ID /bin/bash
      docker exec -it CONTAINER_ID /bin/sh

### setting up a docker network
  if you want two containers to interact on same port then you need to create a docker network
  #### to check all the netwoks
    docker network ls
  #### to create a new docker network
    docker network create NETWORK_NAME

      

    

