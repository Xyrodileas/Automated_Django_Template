# Automated_Django_Template
Automated deployment with Vagrant and Ansible of a Django Template with Bootstrap

[![Bintray](https://img.shields.io/badge/Ansible-2.4-green.svg)]()[![Bintray](https://img.shields.io/badge/Vagrant-2.0-green.svg)]()[![Bintray](https://img.shields.io/badge/Django-2.0.3-green.svg)]()[![Bintray](https://img.shields.io/badge/VirtualBox-5.1-green.svg)]()

# Requirements
Automagie :
- Vagrant
- Ansible
- Virtualbox

Automated Backend :
- mysql with geerlingguy.mysql

Frontend :
- Python3
- Django and his dependencies
- djang-bootstrap
- pip
- Some pip libraries
- facturesoft-frontend

# QuickStart

- Open a command-line interface into the WebbApp folder located into the Vagrant folder.
- Type "vagrant up"
- Wait for Vagrant and Ansible to do their job
- Browse localhost:8080/app/ to access the application

# Automatisation

Vagrant is responsible to provision the required ressource and his network configuration, and call Ansible to manage the configuration of the ressource
Specs :
- Debian 64bits
- Portforwarding on 1321 (backend) and 8000 (frontend)
- ssh enable, possible to ssh into the machine with the command vagrant ssh

Ansible is responsible to manage the configuration of the allocated ressource.
Ansible will do the following:
- Install and configure MySQL
- Install Python3 and Django
- Set up the dependency for the WebApp
- Create the WebApp project and the application
- Configure the webapp for Bootstrap, MySQL

