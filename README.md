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
