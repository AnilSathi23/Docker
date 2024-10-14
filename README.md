# Docker
This repo contains the learnings of Docker

https://docs.docker.com/engine/install/ubuntu/

https://docs.docker.com/desktop/install/windows-install/

docker images
docker image ls
docker run = pull + create

docker pull ubuntu
docker pull nginx

DTR: Docker Trusted Registry
where all the docker images are available

![alt text](image.png)

docker images (all downloded images)
docker pull <image-name>
docker rmi <Image-name>


docker run <image-name>
 docker run -it ubuntu   
 
 -it means interactive terminal

 docker ps
 shows the running containers


 docker ps -a (all running and stopped container)


docker rmi -f nginx (this will forcefully delete the images without worring about the continers refering this image)


Containers is an instance of docker image

docker rm <container-id>

docker stop <container-id>
docker start <container-id>


container take space from Ram
Images takes space from hard disk

docker start container-id

docker run will always create  a new continer

docker exec -it <container-id>

Docker Container Commands

 

1. docker run <image-name>

   docker run -it ubuntu

2. docker ps (running container)

3. docker ps -a (all running and stopped container)

4. docker rm <cont-id>

5. docker stop <cont-id>

6. docker start <cont-id>

7. docker exec -it <cont-id> /bin/bash


delete all containers

docker ps -aq

The following need to be executed in git gitbash for windows
docker rm -f $(docker ps -aq)


Day2

Containers vs Virtual Machines
Build your own Docker image
Tag and image 
Registry (Repository where you can add your docker image)
local vs Remote Repository(Dockerhub)

Apphine is an OS whose size is 7.5 mb

![alt text](image-2.png)

Container size is way less than the actual VM size

Guest OS for VM
Minimum OS for Containers


![alt text](image-3.png)

Responsibility of developer or deveops engineer to make the docker image.




