
# Docker & Kubernetes

A walkthrough Docker&Kubernetes crash course with a summary of basic commands 


## Resources

 - [Docker&Kubernetes-AraBigData](https://youtu.be/PrusdhS2lmo?si=OaSjOlv7VH2nZwV9)
 - [AraBigData-Github](https://github.com/ahmedsami76/AraBigData)


## Getting Started

```bash
 docker image pull <image name>:<version>
```
 by default if version not specified it would pull the latest version.

---

```bash
 docker container create <argument> <image name> <command>
 docker container start <argument> <container id or name>
```

```bash
 docker container run <argument> <image>
```
 'run' command can make up for three commands (image pull , create and start)
 as it pulls image(if not found locally) , create a new container and start container.

---

 To run executable(command) inside a running container 
```bash
 docker exec -it <container> <command>
 docker exec -it nginx bash
```
---
 To stop container
```bash
 docker container stop <container id or container name>
```

 To exit container without stopping
```bash
 Ctrl+p then ctrl+q  
```
---

Listing commands
```bash
 docker image ls 
 docker container ls       #list running containers
 docker container ls --all #list all containers
```
---
## Remove & Delete
```bash
 docker container rm <container id>
 docker image rm <image name>
 docker container rm $(docker container ls -aq) -f    #remove all containers
 docker image rm $(docker image ls -q) -f             #remove all images
```
---
## Images-Deep dive

 To pull unofficial image
```bash
  docker image pull <publisher>/<unofficial image name>:<version>
```

 To rename container and container hostname 
```bash
  docker container run <argument> --name <new container name> -h <new container hostname> <image:version>
  docker container run -it --name alpine -h alp alpine 
```
So alpine linux container shell for example would look like [root@alp] on running instead of [root@2325f9e04787] and container name would be alpine instead of bla-bla names those made up by default.

---

















