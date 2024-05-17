<a name="topage"></a>

# docker_container

# A
# B
# C
# D
   * dictionary etc.
# E
# F
# G
# H
# I
   * Inspect an existing container:
docker inspect <container_id>

# J
# K
# L
   * list currently running containers:
       ```
       docker ps
       ```
   * list all docker containers (status: stop/start):
      ```
      docker ps --a
      ```
   * list all docker containers (status: stop/start):
      ```
      docker ps --all
      ```
# M
# N
# O
# P
# Q
# R
# S
## `start` an existing container:
   * command template:
       ```
       docker start <container_name/container-id>
       ```
   * example: start 1 container-id (5395481d7201)
       ```
       sudo docker start 5395481d7201
       ```
## `stop` an existing container:     
   * command template::
       ```
       docker stop <container_name/container-id>
       ```
   * example: stop 3 container-id (5395481d7201 42bc125f19c3 b60e702047e4)
       ```
       sudo docker stop 5395481d7201 42bc125f19c3 b60e702047e4
       ```
## `stat` - docker container stats
   * command template:
       ```
       docker container stats
       ```
   * output
       ```
      CONTAINER ID   NAME           CPU %     MEM USAGE / LIMIT     MEM %     NET I/O       BLOCK I/O         PIDS
      5395481d7201   some-mariadb   0.02%     76.86MiB / 15.33GiB   0.49%     8.09kB / 0B   4.81MB / 32.8kB   11
       ``` 
   * `ctrl+c` - exit the `stats` window

# T 
# U
# V
# W
# X
# Y
# Z


----


<p align="right">(<a href="#topage">back to top</a>)</p>
<br/>
<br/>
