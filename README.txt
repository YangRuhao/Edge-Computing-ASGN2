Ruhao Yang (21387451)

Docker Hub Links:

- Ubuntu Base Image: https://hub.docker.com/repository/docker/ruhaoyang/group-ubuntu/general

Commands: 
# Pull and run the Ubuntu container
docker run -it username/group-ubuntu bash

# Verify the setup
cat /ASGN2/members.txt  # Should show my name

Docker Images:
For IPC Translator (https://hub.docker.com/repository/docker/ruhaoyang/translator/general):
- Server: docker pull ruhaoyang/translator:server
- Client: docker pull ruhaoyang/translator:client

Commands:
docker network create trans-net
docker run -d --name trans-server --network trans-net username/translator:server
docker run -it --rm --name trans-client --network trans-net username/translator:client


