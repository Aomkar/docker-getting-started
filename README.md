# docker-getting-started

In the terminal go to this project directory and then run the following commands:

('html-test' can be replaced with any name you want...)

docker build -t html-test:v1 . (don't forget the dot at the end)

docker run -d -p 80:80 html-test:v1 (to run the docker image you just built)

THAT'S IT...

Go to localhost:80 in the browser... Voila!!!... Basic html is being rendered through a docker image...

Additional useful commands:
----------------------------

docker images 
    - to list all the docker images. After you build one, check if its accessible via this command

docker ps 
    - to list all the running docker images

docker ps -a
    - to list all the docker images

docker stop [docker_image alias]
    - to stop a running docker image
    - the docker_image alias can be found out with docker ps command
    - you can use CONTAINER ID in place of the alias name. (container id can be found with 'docker ps' command)
