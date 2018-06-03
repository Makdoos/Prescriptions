# Prescriptions
Fedra Prescription is the new and innovative way to demonstrate how Blockchain could ease the way the medical industry works

Follow the documentation to get the demo running on your Mac OS machine. 

1. Install Git: 

To download the latest Git for Mac OS: 
https://sourceforge.net/projects/git-osx-installer/files/ 

click on the downloaded dmg file and run the package by double click on it
.......................................................................................
2. Install NVM - Node Version Manager 

Open the terminal and type the commands bellow: 

- touch ~/.bash profile 
- curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.32.1/install.sh | bash

It might take a while so after It is fineshed, restart your termninal and type : 
- NVM -v 

It should appear the options which means the NVM is installed now on your machine
.......................................................................................
3. Install Node JS 6.10.0 and NPM - via nvm 

type the follow command in your terminal: 

- nvm install 6.10.0 

It might take a while so after the installing finishes, you might verify by type the follow command on your terminal again: 
- node -v 
- node -v 

to see if the both programs are installed properly 

.......................................................................................
4. Docker and Docker composer: 

Download the Docker on Mac here: 
https://docs.docker.com/docker-for-mac/install/#download-docker-for-mac

Mac has already python 2.7 but in case you need to install, following is the link: 
https://www.python.org/downloads/mac-osx/ 

you would need PIP package to install the docker-compose method: 
https://bootstrap.pypa.io/get-pip.py

Open your terminal and go to where get-pip.py location, and execute the python file via command: 
- python get-pip.py 
to verify if the PIP is installed properly, type in your terminal: 
- pip 

Essentials Docker commands you might need: 

- docker ps 
to view all containers are running on your machine 

- docker images 
to view all images are running on your machine 

- docker rm $(docker ps -a -q)
to remove all the containers and to delete them ( you might need if your program stuck at some points and to start fresh again after)

- docker rmi $(docker images -q)
to remove all images 

sometimes the last command won't work, so this command works for me: 
- docker rmi -f 

.......................................................................................
5. Go Lang 

Open your terminal and type the two commands: 

- brew update 
- brew install golang 

Note: you might need to install HomeBrew package if you do not have it already 

Now, you can verify if the installation is done by type the follwing in your terminal:

- go -v 

.......................................................................................
6. Follow the chain code development tutorial 

Now you are all set to follow the original tutorial from the Hyperledger fabric before we proceed to our (Prescription) DEMO  

http://hyperledger-fabric.readthedocs.io/en/latest/chaincode4ade.html#terminal-1-start-the-network

Note : make sure to bring the network down and restart it with every new deployment (new chaincode deployment; new application): 

- docker-compose -f docker-compose-simple.yaml down
- docker-compose -f docker-compose-simple.yaml up








