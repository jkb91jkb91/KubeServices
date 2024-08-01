# Flux(GitOps) repository with Helm charts
<a name="readme-top"></a>  

<!-- ABOUT THE PROJECT -->
## About The Project  
This repository is used as a part of bigger project and have 2 prerequisuites:  


STEPS:  
Prerequisuite step >>>  1) https://github.com/jkb91jkb91/JenkinsCreator  # Creates Jenkins instance with jobs  
Prerequisuite step >>> 2) https://github.com/jkb91jkb91/Jenkins_KubeStarter  # Creates kubeadm kubernetes cluster on EC2 instances  
**Current step  >>> 3) https://github.com/jkb91jkb91/KubeServices**

This repo contains helm charts used to deploy on kubernetes cluster  
Whole repo is meant to create:  
1) working application on kubernetes cluster
2) services used co create full-fledged CICD solution with monitoring on prometheus and grafana
   
<!-- TECHNOLOGIES -->
## Technologies in this repo
* ![Helm](https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white)
* ![Flux](https://img.shields.io/badge/Flux-023042?style=for-the-badge&logo=flux&logoColor=white)
* ![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)

## Technologies under the hood
* ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
* ![Angular](https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white)
* ![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
* ![Memcached](https://img.shields.io/badge/Memcached-5EAF34?style=for-the-badge&logo=memcached&logoColor=white)
* ![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white)
* ![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)
* ![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white)
* ![Cypress](https://img.shields.io/badge/Cypress-17202C?style=for-the-badge&logo=cypress&logoColor=white)
* ![SonarQube](https://img.shields.io/badge/SonarQube-4E9BCD?style=for-the-badge&logo=sonarqube&logoColor=white)

<!-- FOLDER DESCRIPTION -->
## Folder description  
This repo uses GitOps approach with Flux and contains manifests deployed on kubernetes cluster  
Most important files are:  
1) HelmCharts  # HelmCharts folder  
2) Services for HelmCharts application  # Service_Yamls  folder  
3) NFS manifests linked to the POD # Kubernetes_Yamls  
4) jenkins jobs used for: artifactory,sonarqube  # Jenkins_jobs folder, dependencies for CICD services  

<!-- APPLICATION DESCRIPTION -->
## Application description
Application running on kubernetes cluster is working on few microservices:  
1) Angular + Nginx as a frontend  
2) Django + Nginx as a backend  
3) PostgreSQL as main database  
4) Memcached for cache  
5) RabbitMQ for queue  

<!-- CICD SERVICES DESCRIPTION -->
## CICD services description  
Application contains full-fledged CICD system deployed also on cluster that consists of below:   
1) Sonarqube for static code analysis  
2) Jfrog Artifactory to store artifacts  
3) Prometheus to export data  
4) Grafana to visualize data on dashboards  
5) Cypress GUI to display test results  

<!-- AUTHOR -->
## AUTHOR
Email: jakub.g26101991@gmail.com
