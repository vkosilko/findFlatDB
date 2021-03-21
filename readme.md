#installation  

##git  

```
git config --global user.name "Vladimirak"
git config --global user.email "vladimir.kosilko@gmail.com"

ssh-keygen -t rsa -b 4096 ##copy key to github

git remote add origin https://github.com/vkosilko/findFlatDB.git

```

##Packages 

```
wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -
sudo apt-get install apt-transport-https
echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list
sudo apt-get update

sudo apt-get remove docker docker-engine docker.io containerd runc

sudo apt-get install sublime-text git apt-transport-https 

sudo apt-get remove docker docker-engine docker.io containerd runc
sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg \
    lsb-release


curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg

echo \
  "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

sudo apt-get update

sudo apt-get install docker-ce docker-ce-cli containerd.io



```