# Docker tool
A tool to ease the creation of a Docker image with Python libs, it will create a Docker image from base image python:2.7

### How to create a new Docker image with Python libs
You will need to have Docker installed in the machine you are running from

1. Update the requirements.txt in this folder, add the Python libs you want to this file
2. Run the script create_docker_image with first argument to be the new Docker image name:  ``` ./create_docker_image.sh mycompany/image ```
  1. If you need ***sudo*** to run Docker commands, add sudo prefix to last command too :        
      ``` sudo ./create_docker_image.sh mycompany/image ```
3. This is it! you have a new local Docker image!

If you want to share this docker image with other machines/peers , you will need to push it to a Docker registry, for docker hub:

1. Login to Docker Hub: ``` docker login ```
2. Push image: ``` docker push mycompany/image ```