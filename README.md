# docker-wine

A base image for running windows programs on linux

# purpose

Many of my project need a Windows environment to build, it is hard to intergrate Windows build server to our Jenkins CI system, because config a Windows slave is not so easy as we thought.

This image is a base for later work to setup a Jenkins slave machine which can build our code in Linux.

# usage

`docker run --rm -it -e VNC_PASSWORD=newPW -p 5900:5900 mythay/wine /bin/bash`