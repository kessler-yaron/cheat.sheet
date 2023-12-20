<a name="topage"></a>

# brave (internet browser

#### 1) os system update

```sh
sudo apt-get update -y ; apt-get upgrade -y
```

#### 2) install curl

 ```sh
sudo apt install curl -y
```

#### 3) install xxx
  ```sh
XXX
```

#### (*) All net-tools Installation Steps
 ```sh

sudo apt-get update -y ; apt-get upgrade -y

sudo apt install curl -y

sudo curl -fsSLo /usr/share/keyrings/brave-browser-archive-keyring.gpg https://brave-browser-apt-release.s3.brave.com/brave-browser-archive-keyring.gpg

echo "deb [signed-by=/usr/share/keyrings/brave-browser-archive-keyring.gpg] https://brave-browser-apt-release.s3.brave.com/ stable main"|sudo tee /etc/apt/sources.list.d/brave-browser-release.list

sudo apt update -y

sudo apt install brave-browser -y
```

----

<p align="right">(<a href="#topage">back to top</a>)</p>
<br/>
<br/>
