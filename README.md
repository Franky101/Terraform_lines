# Terraform Starting Package
Hi there! ✋

## Introduction
This is a guide to start understanding Terraform. You will find some basic actions that can be done in AWS through Terraform. Simple actions that could take hours are now available in one click.

**Important:** Please exercise caution while using Terraform, as it can have significant consequences on your AWS resources.

## Instructions
1. **Get Started:**
   - Fork this repository to your GitHub account.
   - Clone your forked repository to your local machine.
   - Add your Terraform scripts following the instructions below.

2. **Set up AWS Credentials:**
   To access AWS resources, you need to connect Terraform to an existing AWS profile. If you don't have an AWS profile ready, follow this guide.

   ```go
   # provider.tf
   provider "aws" {
     region   = "<region>"
     profile  = "<your-aws-user>"
   }

3. **Terraform Commands**
    Run the following Terraform commands in your terminal:
    ```bash
    terraform init
    terraform plan
    terraform apply
    ```
     ⚠️**Costs of these deployment**
    We aware that this plan has included EIP (AWS Elastic IP) and NAT GATEWAYS **Are not included in AWS free tier at any point**.


4. When you are finished using your Terraform-managed infrastructure, destroy it with the following command:
    ```bash
    terraform destroy
    ```
    ⚠️**Destroy Infrastructure**
    This command will tear down everything you built. Remember to confirm the destruction to avoid any accidental expenses. Sometimes Terraform may miss destroying some elements, so it's essential to double-check manually in your AWS account.


### Resources

[Watch this video](https://www.youtube.com/watch?v=P_aZ1QucB3E&list=PL184oVW5ERMDGN0a7yowSQiH4qjsTeE5g&index=12) for more insight.


### Have a great day! 🚀
Feel free to reach out if you have any questions or need further assistance. Happy Terraforming! 🚀