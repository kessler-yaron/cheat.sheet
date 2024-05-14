<a name="topage"></a>

# mariadb container

### install `mariadb` docker container
* https://hub.docker.com/_/mariadb

### Install 3 options
1. docker run --detach --name some-mariadb --env MARIADB_ROOT_PASSWORD=my-secret-pw  mariadb:latest
2. docker run --detach --name some-mariadb --env MARIADB_ALLOW_EMPTY_ROOT_PASSWORD=1  mariadb:latest
3. docker run --detach --name some-mariadb --env MARIADB_RANDOM_ROOT_PASSWORD=1  mariadb:latest

### sample #1
```
docker run --detach --name mydb --env MARIADB_ROOT_PASSWORD="!234"  mariadb:latest
```

----

<p align="right">(<a href="#topage">back to top</a>)</p>
<br/>
<br/>
