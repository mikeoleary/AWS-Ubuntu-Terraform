# AWS-Ubuntu-Terraform
Deploys an Ubuntu instance and installs Terraform for when you need a VM that you can quickly spin up and delete.

## Instructions

### Deploy a standalone Ubuntu VM which will be your Terraform client.
1. Deploy a VPC using the <i>vpc.json</i> template. This will create a VPC with a public subnet. <b>Take a note of the name of this stack.</b> 
2. Deploy an Ubuntu machine in AWS using the <i>ubuntu-with-terraform.json</i> template. 
  a. Ensure you install tools by choosing "Yes" at the appropriate input parameter.
  b. Enter the name of your VPC stack to ensure that your VM is deployed to the VPC from the previous step. 
After deploying this template, you will have a public IP address, to which you can SSH. Terraform will be installed, along with the aws cli.

### Configure your AWS credentials.
1. You can follow [these instructions](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html#cli-quick-configuration) to configure the aws-cli. 
