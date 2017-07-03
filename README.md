# Docker
---------------<br>
https://stackoverflow.com/questions/32047660/docker-for-windows-not-working<br>
 docker-machine upgrade<br>
docker-machine restart defaulte
docker version<br>
export DOCKER_API_VERSION=1.21
https://crondev.com/running-docker-behind-proxy/
https://github.com/docker/toolbox/issues/102--proxy
http://containertutorials.com/docker-compose/spring-boot-app.html
https://www.youtube.com/watch?v=6vjo3pMXW7I--war to tomcat using docker hub

https://www.youtube.com/watch?v=FlSup_eelYE
https://mydevgeek.com/spring-boot-docker/<br>
------------------------------------------------------<br>
ADD

The ADD command gets two arguments: a source and a destination. It basically copies the files from the source on the host into the container's own filesystem at the set destination.
==>ADD /my_app_folder /my_app_folder<br>
CMD for Running ur code<br>
# Usage 1: CMD application "argument", "argument", ..
CMD "echo" "Hello docker!"
<br>
FROM<br>
FROM directive is probably the most crucial amongst all others for Dockerfiles. It defines the base image to use to start the build process. It can be any image, including the ones you have created previously. If a FROM image is not found on the host, docker will try to find it (and download) from the docker image index. It needs to be the first command declared inside a Dockerfile.<br>


https://www.digitalocean.com/community/tutorials/docker-explained-using-dockerfiles-to-automate-building-of-images

Steps to run boot app in docker.
mvn clean
mvn install
docker build -t bootdocker .  =>bootdocker is project name.
note:app name shld be in lower case.

For running Spring boot app,below is the code.
docker run -p 8999:8999 bootdocker:dockerfile






