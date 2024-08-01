# Flux(GitOps) repository with Helm charts
<a name="readme-top"></a>  

<!-- ABOUT THE PROJECT -->
## About The Project  
This repository is used as a part of bigger project and have 2 prerequisuites:  
1) https://github.com/jkb91jkb91/JenkinsCreator  # Creates Jenkins instance with jobs  
2) https://github.com/jkb91jkb91/Jenkins_KubeStarter # Creates kubeadm kubernetes cluster on EC2 instances 

This repo contains helm charts used to deploy on kubernetes cluster
<!-- TECHNOLOGIES -->
## Technologies

Technologies:
* ![Helm](https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white)
* ![Flux](https://img.shields.io/badge/Flux-023042?style=for-the-badge&logo=flux&logoColor=white)
* ![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)

<!-- DETAILED DESCRIPTION -->
## Detailed description
This repo uses GitOps approach with Flux and contains manifests deployed on kubernetes cluster  
It has two types of helm files:
1) related to application
2) services for application

Whole repo contains:  
1) Flux configuration and manifests pointing to HelmCharts  
2) HelmCharts  
3) Jenkins jobs  
4) NFS manifests >> Kubernetes_Yamls  
5) Additional Services >> Service_yamls  


<!-- RESULT -->
## Result


<!-- AUTHOR -->
## Author
Email: jakub.g26101991@gmail.com
