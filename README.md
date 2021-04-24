# CEG 3120 Project 4 - Makhmud M

# Project 4 - ReadMe File - Using ECR

## Project Overview
- This project works on our previous project where we hosted a html site using apache. This project we take user docker and "Dockerize" our websites and test them locally. Then we use the Github workflows to automatically trigger an action to push our Docker images directly to our Docker account. 

###  how you installed docker + dependencies (WSL2, for example)
- sudo apt-get update
- sudo apt install docker.io 

Download : Dependencies - > sudo apt-get install apt-transport-https ca-certificates curl software-properties-common

### how to build the container
- docker build -t image:1

###  how to run the container
- docker container run --name containerName -p 80:80 [nginx or alpine]

### how to view the project (open a browser...go to ip and port...)
- Open browser and search localhold:# <- your host ip

## Create ECR

### Process to create
-  Using Amazon ECR console, go to repositories and choose region to create your repo in. Then create your repository. 
-  Build Dockerfile image and push. 

## Configure GitHub Secrets

###  What credentials are needed?
- The Admins Username & Passowrd

###  set secrets and secret names
- To set secrets go to your Github repo, and click the settings tab. On the left side under environments you should see secrets tab. From here you can add GitHub Secrets.

## Configure GitHub Workflow
### variables to change
- List the current working directiories with -> git remote -v

- To set it a git repo use - > git remote set-url origin (link to git)


# Project 4 - ReadMe File - Using DockerHub

## Run Project Locally 

### how you installed docker + dependencies (WSL2, for example)
- sudo apt-get update
- sudo apt install docker.io

- Download : Dependencies - > sudo apt-get install apt-transport-https ca-certificates curl software-properties-common

### how to build the container
- docker build -t image:1

### how to run the container
- docker container run --name containerName -p 80:80 [nginx or alpine]

### how to view the project (open a browser...go to ip and port...)
Open browser and search localhold:# <- your host ip

## Configure AWS CLI
- need AWS IAM user with admin credentials
- how you installed

- how to configure

## Create DockerHub public repo

### Process to create
- on hub.docker.com create an account and head to repositories. On the repositories page click on create repository. You can name and add a description to it as well as connect your github account.

## Configure GitHub Secrets

### What credentials are needed?
- The Admins Username & Passowrd

### set secrets and secret names
- To set secrets go to your Github repo, and click the settings tab. On the left side under environments you should see secrets tab. From here you can add GitHub Secrets.

## Configure GitHub Workflow
### variables to change
- List the current working directiories with -> git remote -v

- To set it a git repo use - > git remote set-url origin (link to git) 


# Extra Credit : Docker Pull

### How To Pull Image With Docker Pull
- Use the command : docker pull (options) (image name):(image tag)
