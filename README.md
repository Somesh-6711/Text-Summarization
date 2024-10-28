# 📝 End to ENd Text-Summarization-Project

## 🛠️ Workflows

1. Update config.yaml
2. Update params.yaml
3. Update entity
4. Update the configuration manager in src config
5. update the conponents
6. update the pipeline
7. update the main.py
8. update the app.py


# 🚀  How to run?
### STEPS:

Clone the repository

```bash
https://github.com/entbappy/End-to-end-Text-Summarization
```
### STEP 01- Create a conda environment after opening the repository

```bash
conda create -n summary python=3.8 -y
```

```bash
conda activate summary
```


### STEP 02- install the requirements
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
Author: Krish Naik
Data Scientist
Email: krishnaik06@gmail.com

```



# 🐳 AWS CI/CD Deployment with GitHub Actions 🚀

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
    - Save the URI: 566373416292.dkr.ecr.us-east-1.amazonaws.com/text-s

	
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

    AWS_ACCESS_KEY_ID=

    AWS_SECRET_ACCESS_KEY=

    AWS_REGION = us-east-1

    AWS_ECR_LOGIN_URI = demo>>  566373416292.dkr.ecr.ap-south-1.amazonaws.com

    ECR_REPOSITORY_NAME = simple-app

# 🛠️ Deployment Steps
Build Docker Image: The source code is containerized using Docker.
Push Docker Image to ECR: The image is pushed to AWS Elastic Container Registry (ECR).
Launch EC2 Instance: The application is deployed on AWS EC2.
Pull Docker Image from ECR: The EC2 instance pulls the latest Docker image from ECR.
Run Docker Container: The Docker image is run on the EC2 instance, hosting the summarizer service.



![Screenshot 2023-11-20 133725](https://github.com/user-attachments/assets/d9a2ed12-de19-48cd-af6a-6b7f997e66b4)
![Screenshot 2023-11-20 133703](https://github.com/user-attachments/assets/6c7553a9-272b-42a2-8c25-d6d7aba783ac)
![Screenshot 2023-11-20 133644](https://github.com/user-attachments/assets/3e5e3751-7ddc-4319-933e-95b39e797881)



### i am a student, i am learning and trying to be batter 


###### Referance: https://github.com/krishnaik06/Text-Summarization-NLP-Project.git
