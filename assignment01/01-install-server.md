# Install Server and Docker


## How to install Server

1. dowload Ubuntu Server to USB
2. Setup and apt-get update to ubuntu server
3. dowload tools that need like vim, ifconfig, git
4. go to https://www.digitalocean.com/community/tutorials/how-to-install-git-on-ubuntu to install git 
    sudo apt update
    sudo apt install git
    git --version
7. git clone https://github.com/sergio11/iot_event_streaming_architecture.git 

## How to install Docker

1. go to https://docs.docker.com/engine/install/ubuntu/
2. Set up Docker's apt repository. and install step by step
    sudo apt-get update
    sudo apt-get install ca-certificates curl
    sudo install -m 0755 -d /etc/apt/keyrings
    sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
    sudo chmod a+r /etc/apt/keyrings/docker.asc
    echo \
    "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
    $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
    sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
    sudo apt-get update
3. install the latest version, run:
    sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
4. Verify that the Docker Engine installation is successful by running the hello-world image.
    sudo docker run hello-world
5. after we install docker we should type command docker login because it need to compose up







