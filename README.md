# docker-compose-fbctf
This docker compose microservice will create an fbctf scoring engine.
## Docker compose services
The docker compose yml creates 3 services using the following containers: 
 - mysql docker container
 - memcached docker container
 - The rafaelfoster/fbctf docker container
## CTF Web-UI Default Username and Password 
 - The default username:password to access the scoring engine Web-UI is admin: fbctf_password.  You can change this password either when bringing up the service via a Dockerfile or after the service has been created.  For more info about changing the default passowrd, please use this Web link: https://hub.docker.com/r/rafaelfoster/fbctf .
## Docker volume for mysql service
 - You will need to create a docker volume for the mysql service so your your game data can persist.  To creat your volume you can execute the following command:
    > docker volume create ctf-data
## Installing the docker container engine and docker compose
 - You will need to install both the docker container engine and docker compose on your Linux virtual machine or server
 - Installing docker engine on ubuntu 20.04: https://docs.docker.com/engine/install/ubuntu/
 - Installing docker compose on ubuntu 20.04: https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-compose-on-ubuntu-20-04
## Starting your docker compose ctf service
 - To start your ctf docker compose service, simply execute the following command in the directory where your fbctf docker-compose.yml file is located:
    > docker-compose up -d 
