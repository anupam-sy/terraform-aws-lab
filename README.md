# Terraform Code
This repository contains Terraform code for resource deployment on AWS Public Cloud.

## Prerequisites:
Below prerequisites must be fulfilled for successful execution of terraform code.

### Software Requirement:
Resources in this repository are meant for use with Terraform 1.0.0 (Check the version using `terraform --version`). If you don't have the compatible version, download it from official Terraform repository.

-   [Terraform](https://www.terraform.io/downloads.html) >= 1.0.0
-   [terraform-provider-aws] plugin = 3.70.0

### Permissions Requirement:
In order to successfully execute the code, you can have a user having "AdministratorAccess". Access can be more fine-grained to follow Principle of least privilege (PoLP).

## Execution:
To execute the Terraform code, go to command prompt, change the directory to your terraform configuration directory and then execute the following commands:

-   Run `[Required] terraform init` to initialize the terraform working directory.
-   Run `[Optional] terraform validate` to check whether configuration is syntactically valid and internally consistent.
-   Run `[Optional] terraform fmt` to rewrite Terraform configuration files to a canonical format and style.
-   Run `[Optional] terraform plan` to preview the execution plan.
-   Run `[Required] terraform apply` to execute the actions proposed in a Terraform plan.
-   Run `[Optional] terraform destroy` to destory the resources defined in your Terraform configuration.

## Reference:
> https://www.terraform.io/cli
> https://registry.terraform.io/providers/hashicorp/aws/latest/docs