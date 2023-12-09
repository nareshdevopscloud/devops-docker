docker inspect image nginx  ### to check images details 

docker images # to check list of images 
docker ps ## to check running containers 

docker ps -a  ## to check both running and stopped containers 

docker pull image <imagename>

docker run -it imagename /bin/bash  --will enter into the container interact terminal 

docker run -dt imagename /bin/bash -we are not enter into the container detach terminal

docker run -dt --name <name> <imagename> /bin/bash (to give csutome name)


contianer will create
docker create <imagename> 
          or
how create container with custom name #####
docker create --name <requiredname> <imagename>


 how to start container#####

docker start <containerid>
          or
docker start <container name>

 how to stop container#####
docker stop <containerid> 
           or
docker stop <container name>

 docker kill comeplete terminated 
docker kill <containername>

To login container #####
docker exec -it <continername or continerid> /bin/bash

1.if you want to come out from connainer without stop give "ctrl+pq"

2.if you give "exit"  container also will stop

docker rm <containername or continerid> ### to remover stopped container 
docker rmi <imagename> ##to delete image 

docker rm -f <continer id> delete runing continer 

docker run -p <HOST_PORT>:<CONTAINER:PORT> IMAGE_NAME  

docker run -dt -p 3000:3000 --name project-2 saturday   #along port expose
