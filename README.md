# Vodafone-Hackathon

## Introduction
Project is divided in 2 repositories : backend,frontend

## Init
To pull backend and frontend submodules and fixing detached HEAD
```shell
git submodule init
git pull --recurse-submodules
cd backend && git checkout master && cd ..
cd frontend && git checkout master && cd ..
```

## Commands
Bring containers up  [-d] to run detached process
```shell
docker-compose up -d
```
Ubuntu: Make sure docker-compose is updated
```shell
sudo docker-compose up -d
```


Bring containers down
```shell
docker-compose down
```

## Troubleshooting
Error:
Starting 5.7-mysql ... error

ERROR: for 5.7-mysql  Cannot start service mysql: driver failed programming external connectivity on endpoint 5.7-mysql (e0725f848118e0cf22afa8d98be7c8cbaf976031f4ef935de649f7420f540acf): Error starting userland proxy: listen tcp 0.0.0.0:3306: bind: address already in use

ERROR: for mysql  Cannot start service mysql: driver failed programming external connectivity on endpoint 5.7-mysql (e0725f848118e0cf22afa8d98be7c8cbaf976031f4ef935de649f7420f540acf): Error starting userland proxy: listen tcp 0.0.0.0:3306: bind: address already in use
ERROR: Encountered errors while bringing up the project.

Fix:
https://stackoverflow.com/a/47541330

------
Error:
Version in “./docker-compose.yml” is unsupported. You might be seeing this error because you're using the wrong Compose file version

Fix:
Use sudo on step 3 and step 4
https://stackoverflow.com/a/49407448
