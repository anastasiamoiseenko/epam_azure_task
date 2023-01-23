## Azure home task for EPAM DevOps course

### Part 1 – Configure application
1. Create a service connection in a Azure DevOps project to your subscription
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_4_service_connecton.png
2.  Find a pet project for the experiments
I have chosen the simple node.js app to practice following after lectures
3. Build your app locally (npm install/run build/run start)
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_3_run_locally.png
4. Create an Azure DevOps repo
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_5_create_a_repo.png
5. Create a branching policy for you application. Added yourself as a reviewer
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_6_dev_branch.png
### Part 2 – Configure a pipeline to deploy infrastructure
Terraform storage account 
1. Create a separate resource group and deploy azure storage account
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_7_rg_and_storage_account.png
2. Create a container with the name “tfstate” and remember the name. use portal settings
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_8_tfstate_container.png
#### Terraform preparation
1. Create another repo to store devops code
2. Create a folder terraform
3. Add app service implementation
4. Integrate application insights with app service
5. Updated backend “azurerm” according to the guide
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_9_terraform.tf.png
6. Run az login or Connect-AzAccount to connect the azure subscription from your local
7. Run terraform apply to deploy infrastructure 
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_10_terraform_apply.png
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_11_terraform_apply_result.png
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_12_terraform_apply_result2.png
#### Create a terraform pipeline
1. Create a yaml pipeline with the following steps: terraform install, terraform init, terraform plan/apply. Plan is an optional one 
2. Inside yaml pipeline add trigger to main branch. The scenario – when main is updated, pipeline should run automatically
3. Added 3 steps – terraform install, terraform init, terraform plan/apply. Plan is an optional one. You may add it as 4th step
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_13_terraform_pipeline.png
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_14_terraform_pipeline_result.png
### Part 3 – Create a deploy pipeline to app service
1. Add yml pipeline to the application folder
2. Your pipeline structure should contain 2 stages. 1st – build, create zip archieve, and publish an artifact. 2nd – download an artifact and deploy it to azure app service
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_15_app_pipeline_result.png
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_16_app_pipeline_result.png
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_17_yaml1.png
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_18_yaml2.png
![Image alt](https://github.com/anastasiamoiseenko/epam_azure_task/raw/main/screenshots/az_19_yaml3.png