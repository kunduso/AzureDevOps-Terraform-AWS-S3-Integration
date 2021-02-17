[![Build Status](https://littlecoding.visualstudio.com/Project-03/_apis/build/status/kunduso.AzureDevOps-Terraform-AWS-S3-Integration?branchName=main)](https://littlecoding.visualstudio.com/Project-03/_build/latest?definitionId=16&branchName=main)
# AzureDevOps-Terraform-AWS-S3-Integration
### In my previous note [Azure DevOps and Terraform to provision AWS S3](https://skundunotes.com/2021/02/14/azure-devops-and-terraform-to-provision-aws-s3/), I listed in detail the steps to be followed to provision an S3 bucket using Azure DevOps and Terraform. I referred to the classic editor in the build definition/azure pipelines. Build and release definitions declared via a classic editor in Azure DevOps, although they have a log/history of change, tend to evolve independently of the evolution of the code repo they support.

### This gap was identified, and Azure DevOps has a solution of storing the build/pipeline definition as a YAML file alongside the code that it is referring to. The benefit of storing the build definition (YAML) along with the code is that the changes to the build definition are versioned in the same repo, so traceability is simpler -whoever is using the repo now has access to the build definition as well, thereby saving time and effort.

### In this repo, I have the azure-pipelines.yaml file along with Terraform configuration files.

### Details listed out under my blog at [Azure Pipelines (YAML) and Terraform to provision AWS S3](https://skundunotes.com/2021/02/17/azure-pipelines-yaml-and-terraform-to-provision-aws-s3/)