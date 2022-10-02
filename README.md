# clo835-assignment1


Clone the repository to a linux environment (AWS Cloud 9 preferred)
initialize git in the locate environment
add and commit the cloned files on the local environment to git
create a repository on github
push the files in the local environment to the created repository on git hub

If you are not using Cloud9 environment, make sure AWS CLI is configured on the environment you are using.
Install the terraform package
navigate to clo835_fall2022_assignment1/terraform_code/dev/instances
run the terraform init, plan and apply commands to deploy the EC2 instance and the ECR infrastrutures

On the git hub platform, go to settings and configure the action secrets to have the AWS Credentials (Acess Key ID, Secret Key and Session Token)
Build the github action workflow to build the docker images, test run the images and push to the ECR repository (Run github action on Deploy_Images_to_ECR.yaml file - this will deploy the images to the ECR repository on AWS).

On the linux environment, ssh into the created EC2 instance. 
update the package and install all required dependencies like docker. 
configure AWS CLI on the instance 
login into the ECR repository
pull the db (DBv0.2) and app (APPv0.2) images in the repository
deploy the db 


login to the created EC2 instance and install updates and docker package
Configure AWS cli on the environement and add the session token to the AWS credentials file
login to the ECR repository
Pull the DB and App images respectively
Run the DB container
Run the App container

