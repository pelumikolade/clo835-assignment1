# clo835-assignment1

Preparation:
Clone the repository to a linux environment (AWS Cloud 9 preferred)
initialize git in the locate environment
add and commit the cloned files on the local environment to git
create a repository on github
push the files in the local environment to the created repository on git hub

Deployment:
If you are not using Cloud9 environment, make sure AWS CLI is configured on the environment you are using.
Install the terraform package
navigate to clo835_fall2022_assignment1/terraform_code/dev/instances
run the terraform init, plan and apply commands to deploy the EC2 instance and the ECR infrastrutures

On the git hub platform, go to settings and configure the action secrets to have the AWS Credentials (Acess Key ID, Secret Key and Session Token)
Build the github action workflow to build the docker images, test run the images and push to the ECR repository.

On the linux environment, ssh into the created EC2 instance. 
update the package and install all required dependencies like docker. 
configure AWS CLI on the instance 
login into the ECR repository
pull the db (DBv1.0) and app (APPv1.0) images in the repository
deploy the db 

This assignment is in 3 Stages and below are the steps to deploy the assignment

1. Create the infrastructure (EC2 and ECR) using terraform from the terraform_code folder
2. Configure github action to have access to the AWS accounnt in the secrets option of the repository
3. Run github action on Deploy_Images_to_ECR.yaml file - this will deploy the images to the ECR repository on AWS
4. login to the created EC2 instance using terraform and install updates and docker package
5. Configure AWS cli on the environement and add the session token to the AWS credentials file
6. login to the ECR repository
7. Pull the DB and App images respectively
8. Run the DB container
9. Run the App container

