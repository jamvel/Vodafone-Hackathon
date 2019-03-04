# Vodafone-Hackathon

## Introduction
Project is divided in 2 repositories : backend,frontend

## Init
To pull backend and frontend submodules and fixing detached HEAD
```shell
git pull --recurse-submodules
cd backend && git checkout master && cd ..
cd frontend && git checkout master && cd ..
```

## Commands
Bring containers up  [-d] to run detached process
```shell
docker-compose up -d
```

Bring containers down
```shell
docker-compose down
```
