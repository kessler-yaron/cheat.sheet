<a name="topage"></a>

# Docker Engine

#### 1) os system update

```sh
sudo apt-get update -y ; apt-get upgrade -y
```

#### 2) install curl

```sh
apt-get install ca-certificates curl -y
```

#### 3) execute permission

```sh
sudo install -m 0755 -d /etc/apt/keyrings
```

#### 4) xxx

```sh
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
```

#### 5) xxx

```sh
sudo chmod a+r /etc/apt/keyrings/docker.asc
```

#### 6) xxx

```sh
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

#### 7) xxx

```sh
sudo apt-get update
```


#### (*) All net-tools Installation Steps

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

<p align="right">(<a href="#topage">back to top</a>)</p>
<br/>
<br/>
