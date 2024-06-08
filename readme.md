# ansible

1) Ansible is openSource 
2) This is 100% Agentless
3) This works both on push and pull mechanism 

### What is the prerequisite for ansible to work?

 ```The only that you need to make sure is that your ANSIBLE NODE should be able to SSH to the nodes that needs configuration management.```


### Ansible can be operated in 2 ways : 

    1) Manual way    ( No Code Approach and it's 100% not recommended )
    2) Automated way ( YAML : Playbooks : 100% recommended approach )

#### Install Ansible :

curl https://gitlab.com/thecloudcareers/opensource/-/raw/master/lab-tools/ansible/install.sh | sudo bash

To ansible, we need to supply the list of Servres that needs to be managed by ANSIBLE and we call that file as INVENTORY file.

    Inventory File 
    Destination Server Username & Password

ansible all -i inv -e ansible_user=centos -e ansible_password=DevOps321 -m shell -a uptime

here -i is inventory -m is module

To do automated way is ansible playbook

