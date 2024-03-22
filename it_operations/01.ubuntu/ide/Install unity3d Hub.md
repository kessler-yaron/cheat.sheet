# Install unity3d Hub.md

## install unity3d Hub
```
sudo apt-get update -y ; sudo apt-get upgarde -y

## add public signing key:
wget -qO - https://hub.unity3d.com/linux/keys/public | gpg --dearmor | sudo tee /usr/share/keyrings/Unity_Technologies_ApS.gpg > /dev/null

## add Unity Hub repository in /etc/apt/sources.list.d:
sudo sh -c 'echo "deb [signed-by=/usr/share/keyrings/Unity_Technologies_ApS.gpg] https://hub.unity3d.com/linux/repos/deb stable main" > /etc/apt/sources.list.d/unityhub.list'

## Update the package cache and install the package:
sudo apt-get update -y ; sudo apt-get upgarde -y
sudo apt-get install unityhub -y
```

### Note: For some systems, you may need to ensure the following:
   * The directory `/usr/share/keyrings` exists.
   * The user or group installing the Hub has write permissions to the `/usr/share/keyrings` directory.
   * The user or group installing Hub has at least read permissions to the resulting file `Unity_Technologies_ApS.gpg.**`

## uninstall unity3d Hub
```
$ sudo apt-get remove unityhub
```
