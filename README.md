# PHP skeleton with docker  - developer environment 

Git repo which includes xdebug and php-fpm and nginx default site configuration
for the project 

## Start your project after clone

```shell
cd <project-dir>/docker
docker-compose-up
```
post acces the webapp http://localhost:8080/ and http://localhost:8080/default.php

## Notables

* xdebug connects with port 90009 ( checkout the `.vscode` dir for debugger launch setting)
* only port 8080 is exposed to
* change `.env.example` to `.env` inside `docker` dirctory to enable xdebug support 