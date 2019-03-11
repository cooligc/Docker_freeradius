# CaptivePortal_Docker


How to use:

     We have made a simple example setup in https://github.com/Media/CaptivePortal_Docker/freeradius. Set the ip-range which   will connect to the server and the server-secret in clients.conf, set the user/password combination in users.

Steps to install Docker and Docker-Compose environment :

   sudo apt update

   sudo apt-get install docker.io

   sudo curl -L "https://github.com/docker/compose/releases/download/1.23.2/docker-compose-$(uname -s)-$(uname -m)" -o      /usr/local/bin/docker-compose

   sudo chmod +x /usr/local/bin/docker-compose


Container Setup : git clone https://github.com/TesMedia/CaptivePortal_Docker && cd CaptivePortal_Docker/freeradius

Start the server: sudo docker-compose up


