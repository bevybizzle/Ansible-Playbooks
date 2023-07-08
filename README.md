# Ansible-Playbooks

## Brief
When I distro-hop I tend to keep installing the same programs. This takes time. Creating Ansible Playbooks to do this for me should save me some time.

## Pre-requisites
First if you don't already have it, you will need to install ansible.
Ansible can be installed on debian/ubuntu based distros by running: 
```
sudo apt-get install ansible -y
```

You will also need to run the following if you want to manage cargo packages:
```
ansible-galaxy collection install community.general
```

## How To Use
Within the same folder as the playbooks if you run:
```
ansible-playbook --connection=local --ask-become-pass install-all-apps.yml
```
Then the playbooks will go ahead and install.

Use this as a template to create your own playbooks for software you constantly install. I use this for distro hopping between linux distributions and trying different debian/ubuntu based distros.

