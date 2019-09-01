# Doker Repo

Just some examples coded by Antonio Bueno <mail@antoniobs.net> powered by www.antoniobs.net

### How to use?

This repo have examples organized by folders :-)

```
- root
   |- Docker-01    <- Example 1
   |- Docker-02    <- Example 2
   .
   .
   .
   |- Docker-NN     <- Example N
```

### Using examples

I recommend use Debian 9.

I'm using:

```
Linux 4.9.0-8-amd64 #1 SMP Debian 4.9.144-3.1 (2019-02-19) x86_64 GNU/Linux
```

You can download your own copy over here: https://www.debian.org/distrib/

### Read me

Please read each readme.md file for each example.

### Donation

Only if you want: https://antoniobs.net/donaciones

### Code

Happy docking!

# Installing Docker On Debian 9

### 1) Install using the repository

```
sudo apt-get remove docker docker-engine docker.io containerd runc

sudo apt-get update

sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg2 \
    software-properties-common

curl -fsSL https://download.docker.com/linux/debian/gpg | sudo apt-key add -

sudo apt-key fingerprint 0EBFCD88

sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/debian \
   $(lsb_release -cs) \
   stable"
```

### 2) INSTALL DOCKER ENGINE - COMMUNITY

```
sudo apt-get update

sudo apt-get install docker-ce docker-ce-cli containerd.io

apt-cache madison docker-ce

sudo apt-get install docker-ce=5:19.03.1~3-0~debian-stretch docker-ce-cli=5:19.03.1~3-0~debian-stretch containerd.io

sudo docker run hello-world
```

Done!

Source: https://docs.docker.com/install/linux/docker-ce/debian/

# Top Docker Commands

### docker ps

You can see a list of your running containers with the command

Usage:

```
sudo docker ps
```

### docker --version

Show the Docker version information

Usage:

```
docker --version
```

### docker info / docker version

Display system-wide information

Usage:

```
 sudo docker info
 sudo docker version
```

### docker image ls

List images

Usage:

```
sudo docker image ls
```

### docker run

Run a command in a new container

usage:

```
sudo docker run hello-world
```









