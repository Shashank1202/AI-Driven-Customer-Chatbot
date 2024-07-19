# AI-Driven-Customer-Chatbot

## Workflows

1. Update config.yaml
2. Update params.yaml
3. Update entity
4. Update the configuration manager in src config
5. update the conponents
6. update the app.py

## Steps to run the project

Clone the repository

```bash
Project reop: https://github.com/Shashank1202/AI-Driven-Customer-Chatbot.git
```

### STEP 01-Create a conda environment after opening the repository

```bash
conda create -m yourenv_name python=3.8 -y
```

```bash
conda activate yourenv_name
```

### STEP 02- Install the requirements

```bash
pip install -r requirements.txt
```
```bash
# Finally run the following command
python app.py
```
Now,
```bash
open up you local host and port
```


```bash
Author: Shashank S
AI Engineer
Email: shashank.s.1202@gmail.com

```
```ini
PINECONE_API_KEY="YOUR KEY"
PINECONE_API_ENV="YOUR ENV"
```

# AWS-CICD-Deployment-with-Github-Actions

## 1. Login to AWS console.

## 2. Create IAM user for deployment

	#with specific access

	1. EC2 access : It is virtual machine

	2. ECR: Elastic Container registry to save your docker image in aws


	#Description: About the deployment

	1. Build docker image of the source code

	2. Push your docker image to ECR

	3. Launch Your EC2 

	4. Pull Your image from ECR in EC2

	5. Lauch your docker image in EC2

	#Policy:

 1. AmazonEC2ContainerRegistryFullAccess

	2. AmazonEC2FullAccess

	
## 3. Create ECR repo to store/save docker image
    - Save the URI: ' '

	
## 4. Create EC2 machine (Ubuntu) 

## 5. Open EC2 and Install docker in EC2 Machine:
	
	
	#optinal

	sudo apt-get update -y

	sudo apt-get upgrade
	
	#required

	curl -fsSL https://get.docker.com -o get-docker.sh

	sudo sh get-docker.sh

	sudo usermod -aG docker ubuntu

	newgrp docker
	
# 6. Configure EC2 as self-hosted runner:
    setting>actions>runner>new self hosted runner> choose os> then run command one by one


# 7. Setup github secrets:

    AWS_ACCESS_KEY_ID: 'Your access key ID'

    AWS_SECRET_ACCESS_KEY: 'your secret access key'

    AWS_REGION: 'your region'

    AWS_ECR_LOGIN_URI: 'your url'.amazonaws.com

    ECR_REPOSITORY_NAME: 'your repo name'
