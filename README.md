# mini-proj-ansible
Ansible Role: Containerized Webapp
=========

This Ansible playbook will Deploy & run Docker Compose project for Webapp instance.

webapp deployment on host machine using ansible playbook from https://github.com/MTDIOP/mini-proj-ansible .

To use it you first have to deploy an ansible machine with a host.

first install playbook from link given earlier : ansible-galaxy install -r roles/requirements.yml

run with command : ansible-playbook -i hosts.yml --ask-vault-password webapp.yml

Role Variables
=========

This role comes with following variables defined in defaults/main.yml:

```
system_user: admin
webapp_name: webapp
webapp_directory: /home/{{ system_user }}/index.html
webapp_port: 80
```
########### HOW TO USE THE ROLE ##############
Create file ansible.cfg

![alt text](images/image.png)

Create group_vars/prod;yml for creadentials files

![alt text](images/image-1.png)

Create hosts.yml file

![alt text](images/image-2.png)

Create roles/requirement.yml to declare src file

![alt text](images/image-3.png)

Create webapp.yml file to use the role
![alt text](images/image-4.png)

Install the role

ansible-galaxy install -r roles/requirements.yml

![alt text](images/image-5.png)

Deploy the webapp

ansible-playbook -i hosts.yml --ask-vault-password webapp.yml
![alt text](images/image-6.png)

Application Access

![alt text](images/image-7.png)

![alt text](images/image-8.png)