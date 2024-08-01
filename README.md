# Kubernetes HELM charts and FLUX
<a name="readme-top"></a>  

<!-- ABOUT THE PROJECT -->
## About The Project  
This repository is used as a part of bigger project and it is triggered by JENKINS JOBS created as prerequsuite here:
https://github.com/jkb91jkb91/JenkinsCreator  
It is going to deploy kubernetes cluster on EC2 intances on AWS  

This repository contains files related to IaC  
-terraform  
-ansible  

additional files:  
  -bashrc  
  -prepare_for_ansible.sh (to get IP and SSH KEY on local machine) 

<!-- TECHNOLOGIES -->
## Technologies

Technologies used to create this site:
* ![Helm](https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white)
* ![Flux](https://img.shields.io/badge/Flux-023042?style=for-the-badge&logo=flux&logoColor=white)
* ![Terraform](https://img.shields.io/badge/Terraform-623CE4?style=for-the-badge&logo=terraform&logoColor=white)
* ![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=for-the-badge&logo=ansible&logoColor=white)

<!-- DETAILED DESCRIPTION -->
## Detailed description

CODE FROM THIS REPO WILL BE TRIGGERED BY THIS JOBS (prerequisuite >>  https://github.com/jkb91jkb91/JenkinsCreator)  
Prerequisuite step will create for us JENKINS instance and bootstrap it with such jobs:  

JOB1 = A_terraform_stack_create.json  
JOB2 = B_ansible_stack_create.json  
JOB3 = C_ansible_stack_delete.json  
JOB4 = D_terraform_stack_delete.json  

   

STEP CREATION
To create the whole stack do:  
manual trigger ONLY JOB1: (JOB1 = A_terraform_stack_create.json >--automatically triggered-> JOB2 = B_ansible_stack_create.json)  

STEP REMOVING
To delete the whole stack do:  
manual trigger ONLY JOB3: (JOB3 = C_ansible_stack_delete.json   >--automatically triggered-> JOB4 D_terraform_stack_delete.json)  

<!-- RESULT -->
## Result

STEP CREATION RESULT = Created kubeadm kubernetes cluster with master and worker nodes being deployed on EC2 AWS instances  
STEP REMOVING RESULT = Removing whole stack from AWS  

<!-- AUTHOR -->
## Author
Email: jakub.g26101991@gmail.com
