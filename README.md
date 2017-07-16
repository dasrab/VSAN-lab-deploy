# VSAN-lab-deploy
vsphere-nsx-lab-deploy

Ansible playbook to automate deployment of vCenter, nested ESXi hosts

Table of Contents

Description
Setup - The basics of getting started with nsxt
Dependencies
[Edit answersfile.yml](#Edit answersfile.yml)
Usage
[Limitations)
Development
Description

This repository will be used to hold an Ansible Playbook to deploy and configure vCenter and nested ESXi VMs

Setup

Validated on Ubuntu 14 deploying vSphere 6.0 and vSphere 6.5

Dependencies

apt-get install sshpass python-pip git 
pip install vim 
pip install pyvmomi 
git clone  https://github.com/dasrab/VSAN-lab-deploy.git

Place the ESXi and VCSA ISOs in /root/ISOs 

Edit answersfile.yml

Edit answersfile.yml according to your infrastructure!

Usage

ansible-playbook deploy.yml

Limitations

Ansible => 2.2 is required 
ESXi version 6.0 and above is supported 
VCSA version 6.0U2 and above is supported 

Development

TODO: External PSC for vSphere 6.5 VMware internal
