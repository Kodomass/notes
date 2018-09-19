### DOCKER commands

* docker image ls
* docker image ls --all (show all images, including intermediate)

* docker container ls
* docker container ls --all (show all containers, including exited)
* docker ps
* docker ps -a

* docker start <container_ID> (start stopped container)
* docker attach <container_ID> (attach local stdio, stderr to a running container)
* docker start -a,--attach (start and attach in one command)

* docker rm <container_ID>
* docker rmi <image_ID>

* docker build -t image:tag [-f docker_filename] .

* docker run -it <image> /bin/bash   (start new container)
* docker run -d -it <image>   (start new container as deamon)
* docker exec -it <container> /bin/bash   (connect to running container)

* docker logs <container>    (print logs)
* docker system df   (show docker disk usage)

