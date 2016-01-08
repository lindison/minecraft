# docker-minecraft
# testing the automated build functions of DockerHub and other things
A nice and easy way to get a Minecraft server up and running using docker. For
help on getting started with docker see the [official getting started guide][0].
For more information on Minecraft and check out it's [website][1].


## Building docker-minecraft

Running this will build you a docker image with the latest version of both
docker-minecraft and Minecraft itself.

    git clone https://github.com/lindison/minecraft/
    cd minecraft
    sudo docker build -t lindison/minecraft .


## Running minecraft


    sudo docker run -d=true -p=25565:25565 -v=/mnt/minecraft:/data lindison/minecraft /start

## Starting and Stopping

    sudo docker start <container_id>
    sudo docker stop <container_id>
