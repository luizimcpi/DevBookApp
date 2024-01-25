## Local Docker Mysql instructions
```
docker pull mysql/mysql-server:latest

docker run -d -p 3306:3306 --name mysql-docker-container -e MYSQL_ROOT_PASSWORD=123456 -e MYSQL_DATABASE=devbook -e MYSQL_USER=user -e MYSQL_PASSWORD=123456 mysql/mysql-server:latest

sudo docker exec -it mysql-docker-container bash

mysql -u root -p
or
mysql -u user -p
Password: 123456

show databases;
use devbook;
show tables;

1 - run api/sql/sql.sql 
2 - run api/sql/dados.sql
```

## Run api
```
go run api/main.go
```

## Api Docs 
File
```
api.http in the root project folder
```

Use rest client plugin vscode
```
humao.rest-client
```