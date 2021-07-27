# DevOps-101

## Introduction
This repository contains an information, questions and exercises on various technical/DevOps related topics.

## Prerequisites

Accounts:

* [MSDN accounts benefits](https://my.visualstudio.com/benefits)

* [Github account](https://github.com/signup)

* Azure account

* Pluralsight account

* Microsoft Learn account

* Docker Hub Account

Software:

* Some linux-based environment

* Azure CLI

* Docker Engine

* Git

## Learning Path

### Linux

https://docs.microsoft.com/en-us/learn/modules/get-started-with-windows-subsystem-for-linux/

https://docs.microsoft.com/en-us/learn/modules/control-azure-services-with-cli/

https://linuxjourney.com/

#### Linux Homework

1. Deploy a Linux environmet (could be a Virtual Machine, Container Instance, Windows Subsystem for Linux etc.)
2. Install some webserver and reconfigure it so it would run on a custom port (like 8088)
3. Configure and apply a custom response page for the webserver (something like "Hello World!")

### Git

https://docs.microsoft.com/en-us/learn/paths/intro-to-vc-git/

https://learngitbranching.js.org/

https://docs.microsoft.com/en-us/learn/modules/introduction-to-github-visual-studio-code/

https://docs.microsoft.com/en-us/learn/modules/use-git-from-vs-code/

#### Git Homework

1. Fork this repository
2. Clone forked repository to your local environment (could be PC, Virtual Machine, WSL etc.)
3. Locally create a new branch and modify README.md file in it (by appending it with "Hello World!" line)
4. Commit and push all changes to remote Github repository (forked one, not original one)

### Containerisation

https://www.ibm.com/cloud/learn/virtualization-a-complete-guide

https://www.ibm.com/cloud/learn/containers

https://www.ibm.com/cloud/learn/docker

https://docs.microsoft.com/en-us/learn/modules/intro-to-docker-containers/

https://www.youtube.com/watch?v=6gJs0F8V3tM

https://www.youtube.com/watch?v=Mvr9jTTnJrU

#### Containerisation Homework

1. Create Dockerfile (base image can be any prefferable Linux image) in which a webserver is installed and started 
2. Build an image from the Dockerfile (for that you'll need installed Docker Engine) and run the container (don't forget to expose port for HTTP)
3. Validate that you can access the webserver
4. Publish your image to your Docker Hub Registry (for that you'll need account in Docker Registry)

### Continuous Integration (CI)

https://aws.amazon.com/devops/continuous-integration/

https://lab.github.com/githubtraining/github-actions:-hello-world

#### Continuous Integration Homework

1. Create a new Github repository.
2. Create and configure Github Action, which builds Dockerfile and publishes it in Docker Hub Registry once every day.

### Azure

#### Intro

https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-fundamentals/

https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/


#### Access and Security

https://docs.microsoft.com/en-us/learn/modules/explore-basic-services-identity-types/

https://devblogs.microsoft.com/devops/demystifying-service-principals-managed-identities/

https://docs.microsoft.com/en-us/cli/azure/create-an-azure-service-principal-azure-cli

https://docs.microsoft.com/en-us/learn/modules/manage-secrets-with-azure-key-vault/

https://docs.microsoft.com/en-us/learn/modules/secure-azure-resources-with-rbac/

#### Access and Security Homework

1. Register a new application in Azure Active Directory.
2. Generate and store a secret for the application.
3. Create a Key Vault and grant access to the application: on resouce level - Contributor role, on Vault level - policy which would allow to create and read secrets.
4. Using non-GUI approach (Powershell, Azure CLI etc.): authenticate to Azure using application's credentials; create a new secret, read it, delete the whole Key Vault. 

#### ARM Templates

https://docs.microsoft.com/en-us/learn/modules/create-azure-resource-manager-template-vs-code/

https://docs.microsoft.com/en-us/learn/modules/deploy-templates-command-line-github-actions/

### DevOps

https://devops.com/the-origins-of-devops-whats-in-a-name/

https://www.ibm.com/cloud/learn/devops-a-complete-guide

https://aws.amazon.com/devops/what-is-devops/#integration

### Infrastructure as Code

https://www.ibm.com/cloud/learn/infrastructure-as-code

https://docs.microsoft.com/en-us/devops/deliver/what-is-infrastructure-as-code

### Programming

https://docs.microsoft.com/en-us/learn/paths/python-first-steps/


### Ansible

https://docs.microsoft.com/en-us/azure/developer/ansible/

https://developers.redhat.com/courses/ansible/getting-started

https://docs.ansible.com/ansible/latest/user_guide/index.html#get

https://developers.redhat.com/courses/openshift-operators/ansible-review

https://developers.redhat.com/courses/ansible/web-server

### Other

https://app.pluralsight.com/labs/detail/3ede6f2e-1eea-406f-89f9-35e8f55b9c23/toc

https://app.pluralsight.com/labs/detail/e417b99b-2afb-44f7-9dfd-6e6b5f120f49/toc
