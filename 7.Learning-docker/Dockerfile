FROM node:slim
WORKDIR /app
COPY . /app
RUN npm install
EXPOSE 3000
CMD node index.js
# docker login
# docker build -t shivam6862/node-app:0.0.1.RELEASE .
# docker container run -d -p 3000:3000 shivam6862/node-app:0.0.1.RELEASE
# docker container ls
# docker container stop <container id>
# docker push shivam6862/node-app:0.0.1.RELEASE
# docker pull shivam6862/node-app:0.0.1.RELEASE





# docker --version {check docker version}
# docker version --format '{{.Server.Version}}'
# docker pull <image name> {pull image from docker hub}
# docker pull postgres {pull postgres image from docker hub}
# NOTE :- docker compose of various layers of images
# docker image ls  {list of images}
# docker image prune {remove unused images}
# docker ps {list of running containers}  
# NOTE :- when you run docker container it will create a new container from image in your local machine
# docker run -d -p 5432:5432 --name postgres postgres {run postgres container}
# docker run -e POSTGRES_PASSWORD=6862 -d -p 5432:5432 --name postgres postgres {run postgres container with password}
# NOTE :- it will create a new container from image in your local machine
# docker stop <container id> {stop container}
# NOTE :- you have to import a image from docker hub and then you can make as many container as you want
# docker run -d -p 5432:5432 --name postgres-old postgres:13.8 {run postgres container with specific version}
# docker container stop <container id> {stop container}
# docker container ls -a {list of all containers}
# docker container prune {remove unused containers}
# NOTE :- prune command will remove all unused containers show be careful
# docker volume ls {list of all volumes in your local machine} 
# docker pull mongo {pull mongo image from docker hub}
# docker run -d -p 27017:27017 --name mongodb mongo {run mongo container}
# docker logs <container id> {check logs of container}
# docker logs -f <container id> {check logs of container in real time}
# docker run -d -p 27017:27017 -e MONGO_INITDB_ROOT_USERNAME=shivam -e MONGO_INITDB_ROOT_PASSWORD=6862 --net mongodb-network --name mongodb mongo {run mongo container with username and password}
# docker network ls {list of all networks}
# docker run -d -p 8081:8081 -e ME_CONFIG_MONGODB_ADMINUSERNAME=shivam -e ME_CONFIG_MONGODB_ADMINPASSWORD=6862 -e ME_CONFIG_MONGODB_SERVER=mongodb --net mongodb-network --name mongo-express mongo-express {run mongo-express container with username and password}





# docker-compose --version {check docker-compose version}
# docker-compose -f docker-compose.yaml up -d {run docker-compose file}
# NOTE:- data persistency is not there in docker-compose file so we have to add volumes in docker-compose file for data persistency 
# docker-compose -f docker-compose.yaml down {stop docker-compose file}





FROM python:3-alpine3.15
WORKDIR /app
COPY . /app
RUN pip install -r requirements.txt
EXPOSE 5000
CMD python app.py
# docker login
# docker build -t shivam6862/python-app:0.0.1.RELEASE .
# docker container run -d -p 5000:5000 shivam6862/python-app:0.0.1.RELEASE
# docker container ls
# docker container stop <container id>
# docker push shivam6862/python-app:0.0.1.RELEASE
# docker pull shivam6862/python-app:0.0.1.RELEASE