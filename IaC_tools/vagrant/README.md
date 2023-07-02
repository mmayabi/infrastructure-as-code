# Introduction to Vagrant

## What is Vagrant?

- open source
- cross-platform
- **Automate the creation and provisioning of VMs (especially for test)**


## Why use Vagrant in IaC?


## Vagrant Installation

If you're using a Linux distribution, it's better to update it first. After that, you'll need tools such as VirtualBox, VMware, or Hyper-V. I chose VirtualBox, which you can install using the following command:

```
apt install virtualbox  # Debian
yum install virtualbox  # Redhat
```

To proceed, you will need to install Vagrant. The best documentation for this can be found on [HashiCorp's website](https://developer.hashicorp.com/vagrant/downloads). 


## Vagrant Commands

```
vagrant init <image>
vagrant status
vagrant up 
vagrant validate
vagrant ssh
vagrant halt
```

Good resources:

- vagrant -h command :)

How to Obtain Vagrant Boxes Offline:

1. Download from [vagrant cloud](https://app.vagrantup.com/boxes/search)
2. Move to server or place you want
3. use this commands:

```
vagrant box add foo-box /path/to/vagrant-box.box
vagrant init foo-box
vagrant up
```

## Learning Resources

- [Learning DevOps](../../IaC_resources/LearningDevOps_MikaelKrief_Packt.md)
