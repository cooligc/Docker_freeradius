# CaptivePortal_Docker


How to use:

     We have made a simple example setup in https://github.com/Media/CaptivePortal_Docker/freeradius. Set the ip-range which   will connect to the server and the server-secret in clients.conf, set the user/password combination in users.

# Steps to install Docker and Docker-Compose environment :

   sudo apt update

   sudo apt-get install docker.io

   sudo curl -L "https://github.com/docker/compose/releases/download/1.23.2/docker-compose-$(uname -s)-$(uname -m)" -o      /usr/local/bin/docker-compose

   sudo chmod +x /usr/local/bin/docker-compose


# Container Setup : 
    git clone https://github.com/TesMedia/CaptivePortal_Docker && cd CaptivePortal_Docker/freeradius

# Start the server: 
    sudo docker-compose up


#### Docker cheat-sheet:

    sudo docker images -list all local stored images
    sudo docker ps     -list all running containers
    sudo docker exec -it containerName bash -get into the particular running container
    sudo docker inspect -f '{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' containername -show ip of that container
    sudo docker container rm -f $(sudo docker container ls -a -q) -delete all containers
    sudo docker container rm <container name> -remove container
    sudo docker system prune -a -delete all local images which are not using by any running container
 
