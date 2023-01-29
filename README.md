# Auto Configuration with Ansible - Demo Basic

Hands-on lab with Ansible

## Diagram

![alt text](/images/hi.jpg "Title")

From Ansible Host Computer connect to 3 VMs to automatically config
DB with Mysql
Web with Apache

## Run
Install Ansible
```sh
 sudo apt update
 sudo apt install ansible
``` 
Test Ansible is working
```sh
ansible all --key-file ~/.ssh/ansible -i inventory -m ping
```
Run automatically config
```
ansible-playbook sample.yml
```
Using --ask-become-pass to using sudo privillege

## Note
sample-before-role.yml is a file I had written before I wrote specific roles