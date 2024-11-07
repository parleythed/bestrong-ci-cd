# bestrong-ci-cd

# Creating CI/CD pipeline for BeStrong 

# Task:
### You will need to:
### 1) Use Trunk Based development flow for the CI/CD https://trunkbaseddevelopment.com/
### 2) Commit your current Terraform code into the main branch of your Github repository
### 3) Create your Azure DevOps organization.
### 4) Request a free Azure agent (If you haven't yet. Request to Microsoft may take 1-2 business days)
### 5) Write your own Azure DevOps Pipeline build flow using YAML syntax and commit it into your GitHub.
### 6) Build and deploy from the the main branch.
### 7) CI/CD pipeline should include the following steps: terrafrom init, terraform validate, terraform plan and terraform apply (manual approval required). CI/CD on PR should include the following steps: terrafrom init, terraform validate and terraform plan.
### 8) Create a pipeline in Azure DevOps from YAML file and deploy infrastructure into Azure Cloud using Terraform in CI/CD. Use Github service connection to access the repo, Azure service principal connection to grant Azure agent the necessary permissions to perform actions on Azure.

## Comminting Terraform code into the main branch of my Github repository.
![Comminting Terraform code into the main branch of my Github repository.](/screenshot/commiting_tf_code.png)

## Created new Azure DevOps organization. The screenshot shows not only new organization, but also the new project.
![Created Azure DevOps organization](/screenshot/organization_and_project.png)

## My Azure DevOps Pipeline build flow using YAML syntax and commited it in GitHub.
![pipeline in Azure DevOps](/screenshot/my_pipeline.png)
![pipeline in GitHub](/screenshot/pipeline_github.png)

## Results of running pipeline
### Explanation of error:
### authorization.RoleAssignmentsClient#Create: Failure responding to request: StatusCode=403 - because the service principal does not have the required permissions to create or manage role assignments in Azure. Need changes of role assignments by manual.
![running pipeline](/screenshot/result.png)

## Full code of pipeline here [pipeline](pipeline.yaml)
