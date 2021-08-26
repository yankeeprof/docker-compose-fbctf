# docker-compose-fbctf
This docker compose microservice will create an fbctf scoring engine.
## docker compose services
The docker compose yml creates 3 services: 
 -- mysql docker container
 -- memcached docker container
 -- The rafaelfoster/fbctf docker container
The default username:password to access the scoring engine Web-UI is admin: fbctf_password.  You can change this password either when bringing up the service via a Dockerfile or after the service has been created.  For more info about changing the default passowrd, please use this Web link: https://hub.docker.com/r/rafaelfoster/fbctf .
