## Learning DevOps

**Title:** [Learning DevOps]  
**Subtitle** [A comprehensive guide to accelerating DevOps culture adoption with Terraform, Azure DevOps, Kubernetes, and Jenkins]
**Author:** [Mikael Krief]  
**Publisher:** [Packt Publishing Ltd]  
**Edition:** [Second - 2022]  

### Overview

This book is divided into 17 chapters that are organized into 5 sections, making it easy to read and learn from. The clear division of topics and concepts ensures that readers can easily follow along and build upon their knowledge in a step-by-step manner. The book's well-structured pipeline makes it a valuable resource for both beginners and experienced learners alike. furthermore, I want to provide brief explanations for each chapter.

#### Section 1: DevOps and Infrastructure as Code

- Chapter 1, The DevOps Culture and Infrastructure as Code practices

    This chapter explains the concepts of CI/CD and IaC, providing a clear and detailed overview with helpful diagrams to aid understanding. While experts may find the material straightforward and can review it quickly, those who are new to the concepts should read it carefully to gain a thorough understanding. Topics in this chapter:

    - Getting started with DevOps
    - Implementing CI/CD and continuous deployment
    - Understanding IaC practices

- Chapter 2, Provisioning Cloud Infrastructure with Terraform

    This chapter is the first piece of the puzzle of this book, which is explained in Chapter 1. This chapter is designed to help you become familiar with Terraform. However, if you want to learn more and use Terraform in practice, you will need to consult additional resources. The Terraform examples are on the Azure cloud. Topics in this chapter:

    - Installing Terraform (manually and by script on all OSs)
    - Configuring Terraform for Azure
    - Writing a Terraform script to deploy an Azure infrastructure
    - Running Terraform for deployment
    - Understanding the Terraform life cycle with different command-line options
    - Protecting the state file with a remote backend

- Chapter 3, Using Ansible to Configure IaaS Infrastructure

    The second piece is the third chapter, which provides a good review of Ansible. It covers concepts such as static and dynamic inventories, playbooks, and vault. While this chapter is a good starting point, it may not provide enough detail for those who are already experienced with Ansible. If you are an expert with Ansible, you can just review the 'Using a Dynamic Inventory for an Azure Infrastructure' section for a quick overview. Topics in this chapter:

    - Installing Ansible
    - Creating an Ansible inventory
    - Executing the first playbook
    - Executing Ansible
    - Protecting data with Ansible Vault
    - Using a dynamic inventory for an Azure infrastructure

- Chapter 4, Optimizing Infrastructure Deployment with Packer

    This chapter is designed to help you improve your Infrastructure as Code (IaC) architecture. In my opinion, this book covers Ansible and Terraform better than Packer, but it does provide a good overview for readers to follow up with additional resources.
    This chapter does not cover the remote integration of Packer and Ansible. Topics in this chapter:
    
    - An overview of Packer
    - Creating Packer templates using scripts
    - Creating Packer templates using Ansible
    - Executing Packer
    - Writing Packer templates with HCL format
    - Using images created by Packer with Terraform

- Chapter 5, Authoring the Development Environment with Vagrant

    If you want to learn Vagrant, start with this chapter. Learn step by step with good examples. It helps you to have a local lab for your test in IaC. Topics in this chapter:

    - Installing Vagrant
    - Writing a Vagrant configuration file
    - Provisioning a local VM with the Vagrant CLI

tags: [CI/CD, Continuous_Deployment, IaC, Terraform, Azure, Ansible, Packer,Vagrant]

#### Section 2: DevOps CI/CD Pipeline

- Chapter 6, Managing Your Source Code with Git
    This chapter provides a thorough introduction to Git and its fundamentals. Additionally, it includes a useful review of working with Azure DevOps as a remote Git repository. The chapter covers Git client installation but does not cover Git server installation. Thanks for covering GitFlow too. Topics in this chapter:

    - Overviewing Git and its principal command lines
    - Understanding the Git process and Gitflow pattern

- Chapter 7, Continuous Integration and Continuous Deployment

- Chapter 8, Deploying Infrastructure as Code with CI/CD Pipelines

tags: [git, gitflow, Azure DevOps]

#### Section 3: Containerized Microservices with Docker and Kubernetes  

#### Section 4: Testing Your Application

#### Section 5: Taking DevOps Further/More on DevOps

### Key Features

- F1
- F2

### Author's Background

- **Name:** Mikael Krief
- **Expertise:** works as a DevOps engineer. For all his contributions and passion, he has received the Microsoft Most Valuable Professional (MVP) award, which Microsoft has awarded him for the last 6 years and he has been nominated and selected as a Hashicorp Ambassador since 2020.
- **Other Works:** In 2019, he wrote the first edition of this book, and in 2020, he wrote Terraform Cookbook (Packt Publishing), and also contributes to many public projects, writes blogs and books, and speaks at conferences.

### Personal Experience

- In this book, Ansible is categorized as a declarative tool, but in most other resources, Ansible is considered to be an imperative tool. In my opinion, Ansible can be used in a declarative way, but it is fundamentally an imperative tool.

### Recommendation
