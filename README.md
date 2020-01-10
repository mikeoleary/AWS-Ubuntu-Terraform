# AWS-Ubuntu-Terraform
Deploys an Ubuntu instance and installs Terraform

## Instructions

1. Deploy a VPC using the <i>vpc.json</i> template. This will create a VPC with a public subnet. <b>Take a note of the name of this stack.</b> 
2. Deploy an Ubuntu machine in AWS using the <i>ubuntu-with-terraform.json</i> template. After deploying this template, you will have a public IP address, to which you can SSH. Terraform will be installed, along with the aws cli.
