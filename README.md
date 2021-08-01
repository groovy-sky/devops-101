# DevOps-101

## Introduction

![](img/logo.png)

This repository is designed to help anyone with very little or no computing background learn the basics of DevOps. Course is self-paced and when you’re finished with it, you’ll know how to manage resouces in Azure Cloud, using Infrastructure as Code approach. 

Learning path is just a collection of publicly available courses, grouped by a specific topic. Some section have homework part - you can use it for a self-evalution. 

if you have any questions regarding this tutorial, please do not hesitate to contact me (using [Reddit](https://www.reddit.com/user/groovy-sky),[Linkedin](https://www.linkedin.com/in/jurijs-fadejevs/) or by pushing pull request to this repository).

## Prerequisites

Accounts:

* [Github account](https://github.com/signup)

* [Microsoft/Azure account](https://azure.microsoft.com/en-us/free/)

* [Docker Hub Account](https://hub.docker.com/signup)

Software:

* Some linux-based environment (like [Ubuntu](https://ubuntu.com/), [Fedora](https://getfedora.org/), [Suse](https://www.suse.com/) etc.)

* Some software for managing Azure (like [Azure CLI](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli), [Azure Powershell](https://docs.microsoft.com/en-us/powershell/azure/get-started-azureps), [Azure Cloud Shell](https://docs.microsoft.com/en-us/azure/cloud-shell/overview) etc.)

* [Docker Engine](https://docs.docker.com/engine/install/)

* [Git](https://git-scm.com/downloads)

* [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)

## Learning Path

### DevOps

![](img/devops.png) 

1. [The Origins of DevOps](https://devops.com/the-origins-of-devops-whats-in-a-name/)
2. [Guide to DevOps](https://www.ibm.com/cloud/learn/devops-a-complete-guide)
3. [DevOps Model from Amazon](https://aws.amazon.com/devops/what-is-devops/#integration)

### Linux

![](img/linux.png)

1. [Running Windows Subsystem for Linux](https://docs.microsoft.com/en-us/learn/modules/get-started-with-windows-subsystem-for-linux/)
2. [Linux Fundametals](https://linuxjourney.com/)

#### Linux Homework

1. Deploy a Linux environmet (could be a Virtual Machine, Container Instance, Windows Subsystem for Linux etc.)
2. Install some webserver and reconfigure it so it would run on a custom port (like 8088)
3. Configure and apply a custom response page for the webserver (something like "Hello World!")

### Git

![](img/git.png)

1. [Introduction to Git](https://docs.microsoft.com/en-us/learn/paths/intro-to-vc-git/)
2. [Learn Git Branching](https://learngitbranching.js.org/)
3. [Introduction to GitHub in Visual Studio Code](https://docs.microsoft.com/en-us/learn/modules/introduction-to-github-visual-studio-code/)
4. [Working with Git in Visual Studio Code](https://docs.microsoft.com/en-us/learn/modules/use-git-from-vs-code/)

#### Git Homework

1. Fork this repository
2. Clone forked repository to your local environment (could be PC, Virtual Machine, WSL etc.)
3. Locally create a new branch and modify README.md file in it (by appending it with "Hello World!" line)
4. Commit and push all changes to remote Github repository (forked one, not the original)

### Python

![](img/python.png) 

1. [What is Python?](https://docs.microsoft.com/en-us/learn/modules/python-introduction/)
2. [LearnPython.org interactive Python tutorial](https://www.learnpython.org/en/Welcome)
3. [Perform mathematical operations on numeric data in Python](https://docs.microsoft.com/en-us/learn/modules/python-datatypes-numeric-operations/)
4. [Optional][Advanced] [An Introduction to Interactive Programming in Python](https://www.coursera.org/learn/interactive-python-1)

### Containerisation

![](img/containers.png)

1. [What is virtualization?](https://www.ibm.com/cloud/learn/virtualization-a-complete-guide)
2. [What are containers?](https://www.ibm.com/cloud/learn/containers)
3. [What is Docker?](https://www.ibm.com/cloud/learn/docker)
4. [Introduction to Docker containers](https://docs.microsoft.com/en-us/learn/modules/intro-to-docker-containers/)
5. [Containers for Beginners](https://youtu.be/6gJs0F8V3tM)

#### Containerisation Homework

1. Create Dockerfile (base image can be any prefferable Linux image) in which a webserver is installed and started 
2. Build an image from the Dockerfile (for that you'll need installed Docker Engine) and run the container (don't forget to expose port for HTTP)
3. Validate that you can access the webserver
4. Publish your image to your Docker Hub Registry (for that you'll need account in Docker Registry)

### Continuous Integration (CI)

![](img/ci.png)

1. [Continuous Integration Explained](https://aws.amazon.com/devops/continuous-integration/)
2. [Create your first GitHub Action](https://lab.github.com/githubtraining/github-actions:-hello-world)

#### Continuous Integration Homework

1. Create a new Github repository.
2. Create and configure Github Action, which builds Dockerfile and publishes it in Docker Hub Registry once every day.

### Azure

![](img/azure.png)

#### Intro

1. [Introduction to Azure fundamentals](https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-fundamentals/)
2. [Create an Azure account](https://docs.microsoft.com/en-us/learn/modules/create-an-azure-account/)
3. [Manage services with the Azure portal](https://docs.microsoft.com/en-us/learn/modules/tour-azure-portal/)

#### Access and Security


1. [Services and identity types of Azure AD](https://docs.microsoft.com/en-us/learn/modules/explore-basic-services-identity-types/)
2. [Service Principals vs Managed Identities](https://devblogs.microsoft.com/devops/demystifying-service-principals-managed-identities/)
3. [Create a service principal](https://docs.microsoft.com/en-us/cli/azure/create-an-azure-service-principal-azure-cli)
4. [Manage secrets with Azure Key Vault](https://docs.microsoft.com/en-us/learn/modules/manage-secrets-with-azure-key-vault/)
5. [Azure role-based access control](https://docs.microsoft.com/en-us/learn/modules/secure-azure-resources-with-rbac/)

##### Access and Security Homework

1. Register a new application in Azure Active Directory.
2. Generate and store a secret for the application.
3. Create a Key Vault and grant access to the application: on resouce level - Contributor role, on Vault level - policy which would allow to create and read secrets.
4. Using non-GUI approach (Powershell, Azure CLI etc.): authenticate to Azure using application's credentials; create a new secret, read it, delete the whole Key Vault. 

#### ARM Templates

1. [Deploy resources using ARM template](https://docs.microsoft.com/en-us/learn/modules/create-azure-resource-manager-template-vs-code/)
2. [Use Azure Key Vault to pass secure parameters](https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/key-vault-parameter?tabs=azure-cli)
3. [Deploy ARM templates by using GitHub Actions](https://docs.microsoft.com/en-us/learn/modules/deploy-templates-command-line-github-actions/)

##### ARM Templates Homework

1. Create a new Key Vault and add a secret with some value, which will be used as virtual machines password
2. Deploy [DNS Forwarder](https://azure.microsoft.com/en-us/resources/templates/dns-forwarder/) with your own parameters file, which for an user password would use Key Vault refference
3. Check the result by logging in VM using a password from the Key Vault

#### Networks

1. [Fundamentals of computer networking](https://docs.microsoft.com/en-us/learn/modules/network-fundamentals/)
2. [Connect on-prem to Azure using VPN Gateway](https://docs.microsoft.com/en-us/learn/modules/connect-on-premises-network-with-vpn-gateway/)
3. [Connect on-prem to Azure using ExpressRoute](https://docs.microsoft.com/en-us/learn/modules/connect-on-premises-network-with-expressroute/)
5. [Design an IP addressing schema](https://docs.microsoft.com/en-us/learn/modules/design-ip-addressing-for-azure/)
6. [Intro to VNet peering](https://docs.microsoft.com/en-us/learn/modules/integrate-vnets-with-vnet-peering/)
7. [Hub and Spoke topology](https://docs.microsoft.com/en-us/learn/modules/hub-and-spoke-network-architecture/2-implement-hub-spoke)
8. [Design and implement private access to Azure Services](https://docs.microsoft.com/en-us/learn/modules/design-implement-private-access-to-azure-services/)

##### Networks Homework

1. Create two VNets with different IP ranges (which doesn't overlap) and a storage account
2. Expose storage account's fileshare privately (using private endpoint) on both networks
3. Establish between networks VNet peering
4. Create two virtual machines - one in the first network with public IP and another in the second network without public IP
5. Connect remotely to publicly available machine and using it connect to the privately available VM
6. From both VMs resolve privately exposed fileshare (using nslookup or any other prefferable way) and validate that in both cases IP is private

#### Serverless

1. [Choose the right integration and automation services in Azure](https://docs.microsoft.com/en-us/azure/azure-functions/functions-compare-logic-apps-ms-flow-webjobs)
2. [Configure Azure Container Instances](https://docs.microsoft.com/en-us/learn/modules/configure-azure-container-instances/)
3. [Publish Azure Functions by using Azure Functions Core Tools](https://docs.microsoft.com/en-us/learn/modules/develop-test-deploy-azure-functions-with-core-tools/)
4. [ Create a Python function in Azure from the command line](https://docs.microsoft.com/en-us/azure/azure-functions/create-first-function-cli-python?tabs=azure-cli%2Cbash%2Cbrowser)
5. [Monitor GitHub events by using a webhook with Azure Functions](https://docs.microsoft.com/en-us/learn/modules/monitor-github-events-with-a-function-triggered-by-a-webhook/)
6. [Create a function on Linux using a custom container](https://docs.microsoft.com/en-us/azure/azure-functions/functions-create-function-linux-custom-image?tabs=bash%2Cportal&pivots=programming-language-python)

##### Serverless Homework

1. Deploy [function for showing your public IP](https://www.serverlesslibrary.net/sample/b85aac2c-4ac5-4c00-9cf6-6c68841c00e5) and check how it works
2. Configure the same function but as a custom Docker container, deploy that image to Azure Container Instance with public IP address and exposed HTTP port and validate the result

### Azure DevOps

![](img/azure_devops.png) 

1. [Introduction to Azure DevOps](https://docs.microsoft.com/en-us/learn/modules/get-started-with-devops/)
2. [Implement CI/CD with Azure DevOps](https://docs.microsoft.com/en-us/learn/modules/implement-ci-cd-azure-devops/)
3. [Host your own build agent in Azure Pipelines](https://docs.microsoft.com/en-us/learn/modules/host-build-agent/)

####  Azure DevOps Homework

1. Create [a new organization and project in Azure DevOps](https://docs.microsoft.com/en-us/azure/devops/organizations/accounts/create-organization?view=azure-devops).
2. Deploy and configure [self-hosted build agent on Azure Container Instance](https://github.com/groovy-sky/azure/blob/master/devops-docker-build-00/README.md#introduction).
3. Use self-hosted agent for [deploying a Python web app](https://docs.microsoft.com/en-us/azure/devops/pipelines/ecosystems/python-webapp?view=azure-devops).

### Ansible

![](img/ansible.png)

1. [Ansible Introduction](https://developers.redhat.com/courses/ansible/getting-started)
2. [Ansible Review](https://developers.redhat.com/courses/openshift-operators/ansible-review)
3. [Run web server using Ansible](https://developers.redhat.com/courses/ansible/web-server)
4. [Ansible User Guide](https://docs.ansible.com/ansible/latest/user_guide/index.html#get)
5. [Configure Ansible on an Azure VM](https://docs.microsoft.com/en-us/azure/developer/ansible/install-on-linux-vm?tabs=azure-cli)

### Ansible Homework

1. Install [Ansible with Azure modules](https://docs.microsoft.com/en-us/azure/developer/ansible/install-on-linux-vm)
2. Choose some ARM template from [Azure Quickstart Templates](https://azure.microsoft.com/en-us/resources/templates/?sort=Popular) and deploy it using [azure_rm_deployment](https://docs.ansible.com/ansible/latest/collections/azure/azcollection/azure_rm_deployment_module.html#azure-rm-deployment-module)

### Infrastructure as Code

![](img/iac.png)

[What is Infrastructure as Code (IaC)?](https://www.ibm.com/cloud/learn/infrastructure-as-code)

### Infrastructure as Code Homework

Configure and deploy [your own IaC](https://github.com/groovy-sky/iaac-demo)

## Next steps

![](img/finish.png)

Congratulations! You have successfully completed this course! Now you can explore Azure by yourself. If you still wondering where to start, check following resources:

* [Azure Tips and Tricks](https://microsoft.github.io/AzureTipsAndTricks/)
* [Small blog about Azure](https://github.com/groovy-sky/azure#introduction)
* [John Savill's Youtube channel](https://www.youtube.com/user/NTFAQGuy)
* [Azure updates](https://azure.microsoft.com/en-us/updates/)
* [Azure Weekly newsletter](https://azureweekly.info/)
