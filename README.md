# ansible-httpd
Ansible script to configure httpd on server

Steps to run the playbook.
##1) add host entry in /etc/ansible/hosts file.

[Apache]

10.0.1.152 ansible_user=ec2-user ansible_ssh_private_key_file=PATH_OF_PEM_FILE

##2) run the playbook

ansible-playbook -i /etc/ansible/hosts -b playbook.yml
