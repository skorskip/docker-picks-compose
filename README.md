# docker-picks-compose
This is a compose file to start the [mysql-picks-database](https://github.com/skorskip/mysql-picks-database) project and the [node-picks-services](https://github.com/skorskip/node-picks-services) project

## Requirements
* Docker
* Docker-compose
* Projects listed

## Prerequistes
* git clone mysql-picks-database project to a folder
* git clone node-picks-services project to the same folder
* have this project in the same folder

## Run
### Build Project
To build the project run in terminal in this project:
```
docker-compose build
```
### Start Project
To run the project run in terminal in this project:
```
docker-compose up
```

### Tear Down Project
To bring down the docker containers run in terminal in this project:
```
docker-compose down
```

Node services can be reached at [http://localhost:3000/](http://localhost:3000/)

## Design Choices
### Using v2.1 Docker-Compose
Using old version of docker-compose to use the `condition` tag to wait for mysql, reference [medium article](https://medium.com/@niratattri/building-a-node-js-application-and-deploying-through-docker-meet-docker-aa8ae677ea12)
