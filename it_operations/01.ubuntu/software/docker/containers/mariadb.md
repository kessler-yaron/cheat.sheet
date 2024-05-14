<a name="topage"></a>

# mariadb container

### install `mariadb` docker container
* https://hub.docker.com/_/mariadb

### download docker mariadb
```
docker pull mariadb
```


### Install 3 options
1. docker run --detach --name some-mariadb --env MARIADB_ROOT_PASSWORD=my-secret-pw  mariadb:latest
2. docker run --detach --name some-mariadb --env MARIADB_ALLOW_EMPTY_ROOT_PASSWORD=1  mariadb:latest
3. docker run --detach --name some-mariadb --env MARIADB_RANDOM_ROOT_PASSWORD=1  mariadb:latest

### sample #1
```
docker run -e MYSQL_ROOT_PASSWORD=YourRootPassword -e MYSQL_DATABASE=YourDatabaseName -p 3306:3306 --name mariadb_container -d mariadb:latest
```

### sample #2
```
docker run -e MYSQL_ROOT_PASSWORD="!234" -e MYSQL_DATABASE="test" -p 3306:3306 --name mariadb_container -d mariadb:latest
```

### sample #3
```
docker run --detach --name mydb --env MARIADB_ROOT_PASSWORD="!234"  mariadb:latest
```

----

<p align="right">(<a href="#topage">back to top</a>)</p>
<br/>
<br/>
