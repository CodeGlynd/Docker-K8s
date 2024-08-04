
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
