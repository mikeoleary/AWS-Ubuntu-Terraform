# AWS-Ubuntu-Terraform
Deploys an Ubuntu instance and installs Terraform for when you need a VM that you can quickly spin up and delete.

## Instructions

#### Deploy a standalone Ubuntu VM with Terraform installed
1. Deploy a VPC using the <i>vpc.json</i> template. This will create a VPC with a public subnet. <b>Take a note of the name of this stack.</b> 
2. Deploy an Ubuntu machine in AWS using the <i>ubuntu-with-terraform.json</i> template. 
  a. Ensure you install tools by choosing "Yes" at the appropriate input parameter.
  b. Select a pre-existing keypair. 
  c. Enter the name of your VPC stack to ensure that your VM is deployed to the VPC from the previous step. 
  
#### Access your VM via ssh
After deploying these templates, you will have an output from the template called "EIP". This is the public IP of your VM. You can connect via SSH, using the private key of the keypair you selected during VM deployment.

#### Configure your AWS credentials.
1. You can follow [these instructions](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html#cli-quick-configuration) to configure the aws-cli. 
