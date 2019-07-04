# Docker-Mysql-8.0
Docker Mysql 8.0 for development environment

## Running mysql
```
docker-compose up
```

To run daemonized
```
docker-compose up -d
```

To stop daemon
```
docker-compose mysql stop
```

## MySql
```
docker exec -it mysql mysql -uroot -p
```

## Bash

It still an alpine machine
```
docker exec -it mysql bash
```

## Aliases
```
alias mysql_start="docker-compose -f ~/projects/Docker-Mysql-8.0/docker-compose.yml up -d"
```

```
alias mysql_stop="docker-compose -f ~/projects/Docker-Mysql-8.0/docker-compose.yml stop"
```

```
alias mysql="docker exec -it mysql mysql -uroot -p"
```

## Sha1 Error
```
ALTER USER 'user'@'%' IDENTIFIED WITH mysql_native_password BY 'password';
```