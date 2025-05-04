# CICD_Jenkins_Argocd
java pipeline for java based application using -maven-sonarqube-argocd-helm-k8s

![image](https://github.com/user-attachments/assets/5ad73434-3693-43f2-8e8d-623caaaf068b)

Execute the application locally and access it in the browser

I have gitclone the java application and executed maven targets to generate the artifacts

Built the Docker Image and Accessed the application locally.

![image](https://github.com/user-attachments/assets/cc836dd6-b8eb-4005-a99e-6664b537a1d0)

![image](https://github.com/user-attachments/assets/15f53311-0bcb-4d9f-958e-bc4892cdf931)

![image](https://github.com/user-attachments/assets/6316af02-c50a-45a2-b49c-c22850f3a143)

![image](https://github.com/user-attachments/assets/8eb6ca00-91b6-4061-8a9b-dabe1ea18f5f)

![image](https://github.com/user-attachments/assets/def75c0f-669f-4ddf-a7ca-c6aac689c7f3)

Installation of Ec2 Instance

![image](https://github.com/user-attachments/assets/1858f494-9025-4619-a569-a745375543ce)

Install Jenkins

![image](https://github.com/user-attachments/assets/4b99601c-bb35-4170-b0b5-d9ab01c73102)

Change the Inbound security groups as by default jenkins not accessible by external world. open port 8080 in Inbound rules.

![image](https://github.com/user-attachments/assets/2c516cf2-b7a1-4b8e-9c3e-ea423d9b5af2)

![image](https://github.com/user-attachments/assets/307baf9e-57a8-43f1-b7bb-3cc546638360)

Install Docker pipeline plugin

Install SonarQube scanner plugin

![image](https://github.com/user-attachments/assets/4c055a1b-072c-4851-8962-2a564932998b)

Install sonarserver in ec2 instance

![image](https://github.com/user-attachments/assets/9055ab08-4f16-44f4-b9ef-d7735c1093a9)

![image](https://github.com/user-attachments/assets/5b1b7503-acb0-4326-b21f-bc493d04a912)

![image](https://github.com/user-attachments/assets/60611855-ddd4-4f8a-bd63-26e7e3e0e3f6)

connect sonarqube with jenkins

![image](https://github.com/user-attachments/assets/3f2b9cdb-68d1-40ee-b2d4-7a14080bd7c9)

Install Docker in ec2 Instance and restart jenkins

![image](https://github.com/user-attachments/assets/eb342276-8c2e-4b67-9900-7d2586538036)

Install minikube in the terminal

![image](https://github.com/user-attachments/assets/b376f29d-2059-4bc4-8d3f-323682b5d7db)

Install Argocd operator on kubernetes

![image](https://github.com/user-attachments/assets/b737a395-9650-44bb-9ba6-415a61baa4cb)

![image](https://github.com/user-attachments/assets/9e56e83e-7f94-4995-8760-0eac246e1a23)

I have run the Jenkins pipeline, got lot of issues with pipeline. I have done troubleshootings with volumes, versions 

Jenkins is trying to run Docker CLI commands, but docker is not available inside that container.

Even though you switched agent any for the Docker stage, because you're in a script block and used sh, it’s possibly executing within the original container context.

Sonarqube is running good.

![image](https://github.com/user-attachments/assets/6795b12e-6d8b-40dd-9ed4-22d3bfa2365d)

![image](https://github.com/user-attachments/assets/2ab4b430-3ee1-44e5-ae49-e3e8a5a5e9fe)

Argocd operator installed and get pods 

![image](https://github.com/user-attachments/assets/e243b6a8-514c-462d-aa02-0087bc45d0c9)

![image](https://github.com/user-attachments/assets/c1f01737-2169-482c-bccd-339ec98c13d7)

![image](https://github.com/user-attachments/assets/d803e267-46ad-4db6-82a1-99babab0055c)


























