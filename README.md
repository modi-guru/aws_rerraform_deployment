# terraform-aws-deployment.
-------------------Serverless Baseline AWS Infrastructure with Terraform and GitHub Actions--------------------

This repository contains the code for deploying a baseline AWS infrastructure using Terraform and GitHub Actions. The infrastructure consists of two EC2 instances in separate availability zones, and a VPC with two subnets and a security group. The deployment is done using Terraform, and the GitHub Actions workflow is used to automate the deployment process.


*Getting Started*


--------------------------------------------Prerequisites--------------------------------------------------------


- AWS account with appropriate credentials and permissions.
- GitHub account for using GitHub Actions.


-----------------------------------------------Setting Up--------------------------------------------------------



Fork this repository.
Open the variables.tf file and update the values as per your requirement.
Set up the AWS credentials using settings and add the AWS_ACCESS_KEY_ID and AWS_SECRET_ACCESS_KEY environment variables.



---------------------------------------------Deployment-----------------------------------------------------------



Follow these steps to deploy the baseline AWS infrastructure:

1. Clone this repository to your local machine.

2. Set up your AWS credentials by configuring environment variables.

3. Update the `variables.tf` file to customize the deployment settings such as region, CIDR blocks, AMI ID, instance types, etc.

4. Commit your changes and push them to your GitHub repository.

5. Create a new GitHub Actions workflow by adding the necessary deployment steps using the `.github/workflows` directory.

6. The GitHub Actions workflow will be triggered automatically and will deploy the infrastructure to your AWS account.

7. Monitor the workflow execution and verify the successful creation of the VPC, subnets, security group, and EC2 instances in your AWS account.



--------------------------------------------Customization-------------------------------------------------    

Feel free to customize the deployment according to your specific requirements. You can modify the Terraform configuration files (`main.tf` and `variables.tf`) to add or remove resources, adjust networking settings, security group rules, etc.


-------------------------------------------Repository Structure---------------------------------------------


The repository contains the following files:

main.tf: Terraform code for creating the AWS resources.
variables.tf: Input variables for the Terraform code.
.github/workflows/deploy.yml: GitHub Actions workflow file for deploying the infrastructure.


----------------------------------------Contributing-----------------------------------------------------------


Contributions to this repository are always welcome! If you have any suggestions or improvements, feel free to create an issue or a pull request.


-----------------------------------------------License---------------------------------------------------------


This project is licensed under the MIT License - see the LICENSE file for details.


----------------------------------------------------------------------------------------------------------------------
