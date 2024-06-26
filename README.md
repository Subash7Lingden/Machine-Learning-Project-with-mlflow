# Machine-Learning-Project-with-mlflow

## Workflow
1. Update config.yaml
2. Update schema.yaml
3. Update params.yaml
4. Update the entity 
5. Update the configuration manager in the src config
6. Update the components
7. Update the pipeline
8. Update the main.py
9. Upadata the app.py

# How to run the project

### Steps:

Clone the repository
~~~bash
https://github.com/Subash7Lingden/Machine-Learning-Project-with-mlflow
~~~

### Step 01 - Create a conda environement after opening the repository
~~~bash
conda create -n mlproj python=3.8 -y
~~~

~~~bash
conda activate mlproj
~~~

### step 02 - Install the requiements
~~~bash
pip install -r requirements.txt
~~~

~~~bash
# Finally run tht following command
python app.py
~~~
Now,
~~~ bash
open up your local host and port
~~~

## MLflow
[Documentation](https://mlflow.org/docs/latest/index.html)

### cmd
- mlflow ui

### dagshub
[dagshub](https://dagshub.com/)

MLFLOW_TRACKING_URI=https://dagshub.com/Subash7Lingden/Machine-Learning-Project-with-mlflow.mlflow \
MLFLOW_TRACKING_USERNAME=Subash7Lingden \
MLFLOW_TRACKING_PASSWORD=e47cb2181458071797d31f2e25e11e1defd6bd99 \
python script.py

Run this to export as env variables:

~~~bash
set MLFLOW_TRACKING_URI = https://dagshub.com/Subash7Lingden/Machine-Learning-Project-with-mlflow.mlflow

set MLFLOW_TRACKING_USERNAME = Subash7Lingden

set MLFLOW_TRACKING_PASSWORD = e47cb2181458071797d31f2e25e11e1defd6bd99

~~~


AWS -CICD-Deployment-with-Github-Actions

# 1. Login to AWS console
# 2. Create IAM user for deployment (identity access managemet)

    # with specific access 
        a. EC2 access: it is virtual machine
        b. ECR: Elastic Container registry to save your docker image in aws

    # Description: About the deployment
        a. Build docker image if the source code
        b. Push your docker image to ECR
        c. Lunch your EC2
        d. Pull Your image from ECR in EC2
        e. Lunch your docker image in EC 

    # Policy:
        a. AmazonEC2CountanerRegitstyFullAccess
        b. AmazonEC2FullAccess

# 3. Create ECR Repo to store/save docker image (elastic container registry)
- Save the URI: 

# 4. Create EC2 machine (Ubuntu)

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




## About MLflow 
MLflow

 - Its Production Grade
 - Trace all of your expriements
 - Logging & tagging your model





