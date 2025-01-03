# ansible-scripts
Ansible scripts for automated Docker, Minikube, Kind deployments in EC2


Prerequsites:
python 3.8x version installed and available
Ansible version 2.13.x
OS: tested on AWS EC2 AMI

Ansible Galaxy Role: gantsign.minikube

<h2> Steps to Run </h2>

1) Clone the repo
2) Pull the galaxy role
   ansible-galaxy install gantsign.minikube
   ansible-galaxy list ( you see the role listed in the output )


3) Run below to install docker and minikube
   ansible-playbook -i localhost, minikube-playbook.yml --skip-tags kind

5) Run below to install docker and kind
ansible-playbook -i localhost, minikube-playbook.yml --skip-tags minikube
