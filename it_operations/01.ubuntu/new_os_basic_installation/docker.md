<a name="topage"></a>

# Docker Engine

## `A. Set up Docker's apt repository`

#### 1) os system update

```sh
sudo apt-get update -y ; apt-get upgrade -y
```

#### 2) install curl

```sh
sudo apt-get install ca-certificates curl -y
```

#### 3) execute permission

```sh
sudo install -m 0755 -d /etc/apt/keyrings
```

#### 4) PGP public key block

```sh
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
```

#### 5) OS permission PGP public key block

```sh
sudo chmod a+r /etc/apt/keyrings/docker.asc
```

#### 6) Add the repository to Apt sources

```sh
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

#### 7) os system update

```sh
sudo apt-get update
```

#### (1-7) Set up Docker's apt repository - All Steps

 ```sh
# Add Docker's official GPG key:
sudo apt-get update -y ; apt-get upgrade -y
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc

# Add the repository to Apt sources:
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update
```

----

## `B. Install the Docker & Test installation`

#### 1) Install the Docker packages (latest version)

```sh
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin -y
```

#### 2) Test Docker Engine installation `hello-world` image.

```sh
sudo docker run hello-world
```

#### 3) docker version

```sh
sudo docker --version
```

#### 4) docker exists images

```sh
sudo docker images
```

----

## `C. Install the Docker Desktop`

#### 1) Install gnome-terminal (must)

```sh
sudo apt install gnome-terminal
```

#### 2) Download docker-desktop 

##### Download latest DEB package (not latest version)

```sh
https://desktop.docker.com/linux/main/amd64/137060/docker-desktop-4.27.2-amd64.deb?utm_source=docker&utm_medium=webreferral&utm_campaign=docs-driven-download-linux-amd64&_gl=1*1l0hx06*_ga*MTE5NTYxMjQxNy4xNzA4NjYyMTU5*_ga_XJWPQMJYHQ*MTcwODY3MTgwMi4zLjEuMTcwODY3Mjc0NS42MC4wLjA.
```

##### Download latest DEB package  (latest version)

```sh
https://docs.docker.com/desktop/install/ubuntu/#install-docker-desktop
```

#### 3) os system update

```sh
sudo apt-get update -y ; apt-get upgrade -y
```

#### 4) os system update

##### example - template
```sh
sudo apt-get install ./docker-desktop-<version>-<arch>.deb
```

##### example
```sh
sudo apt-get install ./docker-desktop-4.27.2-amd64.deb
```

----

todo:
* docker path
* create a new docker image
* start/stop docker image
* copy + past docker image
* erase docker image
* uninstall docker

----


<p align="right">(<a href="#topage">back to top</a>)</p>
<br/>
<br/>
