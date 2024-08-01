# Flux(GitOps) repository with Helm charts
<a name="readme-top"></a>  

<!-- ABOUT THE PROJECT -->
## About The Project  
This repository is used as a part of bigger project and have 2 prerequisuites:  
1) https://github.com/jkb91jkb91/JenkinsCreator  # Creates Jenkins instance with jobs  
2) https://github.com/jkb91jkb91/Jenkins_KubeStarter # Creates kubeadm kubernetes cluster on EC2 instances 

This repo contains helm charts used to deploy on kubernetes cluster
Whole repo is meant to create:  
1) working application on kubernetes cluster
2) services used co create full-fledged CICD solution with monitoring on prometheus and grafana
   
<!-- TECHNOLOGIES -->
## Technologies
* ![Helm](https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white)
* ![Flux](https://img.shields.io/badge/Flux-023042?style=for-the-badge&logo=flux&logoColor=white)
* ![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)

<!-- DETAILED DESCRIPTION -->
## Detailed description  
This repo uses GitOps approach with Flux and contains manifests deployed on kubernetes cluster  
Most important files are:  
1) HelmCharts  # HelmCharts folder  
2) Services for HelmCharts application  # Service_Yamls  folder
3) NFS manifests linked to the POD # Kubernetes_Yamls  
4) jenkins jobs used for: artifactory,sonarqube  # Jenkins_jobs folder, dependencies for CICD services  

<!-- RESULT -->
## Result


<!-- AUTHOR -->
## Author
Email: jakub.g26101991@gmail.com
