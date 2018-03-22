---
title: bioinformatics workshop dockerisation
author: Elise Gould
date: '2018-03-21'
categories:
  - workshop
  - computational skills
tags:
  - data science
  - reproducibility
  - containerisation
  - docker
slug: bioinformatics-workshop-dockerisation
header:
  caption: ''
  image: ''
---

Slides are here: [http://melbournebioinformatics.github.io/MelBioInf_docs/tutorials/docker/media/index.html#47](http://melbournebioinformatics.github.io/MelBioInf_docs/tutorials/docker/media/index.html#47)

Docker: libraries and operating system included as well (as application).
ALl dependencies distributed. AND docker containers are cross-platform. == Portable.
Distributable: can store images on the docker cloud.

Docker containers can't access host-system's files (good for security), but limits some use-cases (especially where command line utilities used).

Docker containers are very lightweight (no overhead like what virtual machines have). Docker can share libraries... so if have 3 containers running ubuntu, they all share this code, whereas VM's have to have 3 versions, one for each instance.

What is the differnce between images and containers?
docker image --> container.
akin to: class --> object.
 
# Running docker containers

**Run a container**
`docker run <image>` main command you'll be using in docker.

**Finding iages: **
`docker images` lists all the local images

*A note on flags:*
Flags coming before the iamge name act on the container, those coming after the image name act on the image.

**Port mapping:**
If you want to use a web-app inside a container, then you need to map the ports inside the host to the ports inside docker -- docker doesn't have automatic access to any ports on the host.

`-p 80:8080` Before the colon, is the host port (e.g. on your computer, or in this case the instance which we've ssh'd into), after the colon is the port inside the container.

**docker processes:**

`docker ps` ps as in processes. This lists the containers currently running and the ports on the host and on the container where they are listening in on each other.

Note to kill any process in the foreground shell you can hit `ctrl+c`.

`docker ps -a` will show you terminated containers.

**Running in 'detached' mode**

use the `-d` flag as an argument to `run` to let the process run in the background, this gives you access to the shell. If you need to kill a docker process running in detached mode you run the following:

`docker stop <process ID>`, which you can obtain from the command `docker ps` (you don't have to use the full ID generated when you've run the image).

## Giving docker containers access to files

Two main methods, one using binding, and two using volumes.
You might like to do this if you need to save output on a host system (because when you kill a container, any outputs inside the container are also lost). You also might like to give it data to process.

**Volume**

Create filespaceon the host, that the host doesn't have access to, that only the image can access.

**Binding**
If you want access, via the host, then you should use a bind mount.
Note that bind mounts only accept absolute filepaths (i.e. starts with a slash), not relative filepaths.

Note that you can only run `-v` when you are creating a container. You can't run it on an already running container...

## Running commands on already running containers

`Exec` command, runs a command inside a container, once it's running.
`docker exec <CONTAINER ID> <COMMAND>`
e.g. `docker exec bd2ac6cce96f ls`
`docker exec -it bd2ac6cce96f bash` run interactive bash sessions inside a container -- allows you to run a container interactiveyl!!



# Building your own images

You build an image with a docker file. A bit like a shell script or a yaml file.

The main commands inside a docker file are:
`FROM`: Start with Ubuntu, Galaxy, any image... can be anything. Your image inherits form them. Can find an image close to what you want, and then alter it with a few commands to get what you want.
`RUN`: Executes any shell command.
`COPY`: Copies some files from host to image. Very important because otherwise is just the basic downloaded image. You want your files form your repo in there for example. 
`ENTRYPOINT`: executable file that is run when you start a docker image
`WORKDIR`: Sets the working directory, a lot like `cd`

**A note on building images:**

Docker saves the state of the image after each line... SO this helps when building your image, identifying WHERE things are going wrong. This is good, so that if your docker image doesn't build due to some error, you don't have to start building the image from scratch all over again - saves time.


Note that you have to MOVE INTO the directory where you've downloaded freebayes 
then you have to think about installing...
Github file says use sudo... but we don't have to because Docker runs by root, with admin priveleges.
you have to run make

Once you've made the dockerfile, you have to create the image, using `docker run`

# Security & HPC

Don't give people docker access if you don't want the user to access all the files on the system (there are exploits to allow this).

There are alternatives to docker, e.g. [Singularity](http://singularity.lbl.gov/).

