# DockerLearning

Docker solves the problem of inconsistent environments by providing lightweight, portable containers that ensure applications run the same across different systems. It simplifies the deployment, scaling, and management of applications by isolating them in containers with all necessary dependencies.

### Container 
A container in Docker is a lightweight, portable, and isolated environment that packages an application along with its dependencies, ensuring it runs consistently across different systems.

### cmd
 docker -v          ->for version checking
 
 docker run -it demo        ->for running a container which  will have demo image  -it stands for interactive tty
 
 cntrl+D        ->to close the container
 
docker container ls          -> this will show all the working contaners of that docker image

linux commands work on docker (ls,cd,mkdir)

docker start       -> to start the already made container

docker stop       -> to stop the already made container

docker exec -it        -> to excute completely in an isolated container 

docker run -it <image_name>

docker exec <container_name> >command>

### Images
Images are OS on which containers run.
custom image can be made based on the resources and tools required.
(Docker images are lightweight, read-only templates used to create containers. They include the application code, runtime, libraries, and dependencies needed to run an application.)

(hub.docker.com) is where the docker gets its info if needed kinda like github for docker. If docker does not find any image or anything it will search from this hub only.

![image](https://github.com/user-attachments/assets/7910c58d-546f-487b-bd21-5f09ea283e89)

### Port Mapping
Port mapping in Docker allows you to expose a container's internal port to the host machine, enabling communication with the container. It is done using the `-p` option in the `docker run` command.
cmd example - docker run -p 8080:80 nginx

### Containerize Nodejs Application with Docker
 make a Dockerfile (Keep the name of the file same)
 refer to the file Dockerfile
 to run it type -> docker build -t youtube-nodejs . 
 (NOTE: Here the -t means tag and . means the dockerfile is in the current folder directory)
