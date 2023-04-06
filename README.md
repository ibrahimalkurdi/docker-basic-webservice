# Docker Basic Webservice:
This an docker image which will contain nginx server build on top of alpine.|
The html directory will live the content of your web service.
The web service will be exposed on port 8000 on the host machine.

## Build image, push and run it:
```
docker login # Your docker hub account.
docker build -t <image name> -f Dockerfile_homework .
docker push <image name>
docker run -d --name my_assingment -v ${PWD}/html:/usr/share/nginx/html -p 8000:80 <image name>
```
## To run it from dockerhub without build:
```
docker run -d --name my_assingment -v ${PWD}/html:/usr/share/nginx/html -p 8000:80 ibrahimalkurdi/u_assignment
```
To check the main page of the web service, click on this link:
http://localhost:8000

