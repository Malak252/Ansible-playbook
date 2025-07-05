## Ansible-playbook & Jenkins

## Ansible-playbook
ansible-playbook -i inventory frontend.yml

ansible-playbook -i inventory docker.yml


## Setup instructions used to intgrate the 3 machine togther and SSH configuration

ssh-keygen

copy the generated public key and add it to your machine 

on AWS : Network and security > key pairs > action > import keypair > paste yours 

get back and test it on your VM

ssh ubuntu@your.machine.ip

now you can access your machine ssh

screenshoots directory : https://github.com/Malak252/Ansible-playbook/tree/main/screenshoots

## Jenkins

I have created Pipline to use the Jenkinsfile with following stages:
stage1: Build the dockerfile
stage2: Push created Image to my registry 
stage3: connect to Production machine and Deploy the pushed Image on it
Trigger: use webhook to trigger in case Only pull request opned to main and in case merge
