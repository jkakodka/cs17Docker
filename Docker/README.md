## CS17 DOCKER container

##CREATING CS17 DOCKER CONTAINER ON YOUR MACHINE
1. Download and install Docker from here https://www.docker.com/get-started/

2. From this directory,run this command ./cs17-build-docker
    It will take a while for the first run as it pulls the base image(alpine linux) from DockerHub and configures your docker container. Any subsequent runs should be relatively faster. The container is based on alpine linux image and already has node and ReasonML installed.

    The cs17-build-docker is a wrapper script for building docker image based on the Dockerfile from this directory. 

3. In the src directory , you have a script called cs17-run-docker uses the image you built and runs the container environment on your machine.