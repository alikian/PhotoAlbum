#Photo Album

[![Build Status](https://travis-ci.org/alikian/PhotoAlbum.svg?branch=master)](https://travis-ci.org/alikian/PhotoAlbum)

## Build
Use following command to build jar file (maven 3 or higher required):

mvn clean install

## Run
Use following command to run:
``` 
java -jar target/photoalbum-0.0.1-SNAPSHOT.jar
```
At startup application will create tables and also download data

Open browser at:
http://localhost:8080/

Swagger Documentation
http://localhost:8080/swagger-ui.html

## Docker

Build docker image:
```
maven clean install dockerfile:build
```
It will build it under alikian/photoalbum:latest
```
docker run -p 8080:8080 -t alikian/photoalbum 
```


Pull it from Run it in docker.io hub:
```
docker pull alikian/photoalbum:latest
docker run -p 8080:8080 -t alikian/photoalbum 

```