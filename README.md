# mini-proj-ansible
Ansible Role: Containerized Webapp
=========

This Ansible playbook will Deploy & run Docker Compose project for Webapp instance.

webapp deployment on host machine using ansible playbook from https://github.com/MTDIOP/mini-proj-ansible .

To use it you first have to deploy an ansible machine with a host.

first install playbook from link given earlier : ansible-galaxy install -r roles/requirements.yml

run with command : ansible-playbook -i hosts.yml --ask-vault-password webapp.yml