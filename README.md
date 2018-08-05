# docker_exercise

# Build image, push and run it:
```
docker login # Your docker hub account.
docker build -t <image name> -f Dockerfile_homework .
docker push <image name>
docker run -d --name my_assingment -v ${PWD}/html:/usr/share/nginx/html -p 8000:80 <image name>
```
# To run it from dockerhub without build:
```
docker run -d --name my_assingment -v ${PWD}/html:/usr/share/nginx/html -p 8000:80 ibrahimalkurdi/u_assignment
```
