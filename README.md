# ansible-httpd
Ansible script to configure httpd on server

Steps to run the playbook.
1) add host entry in /etc/ansible/hosts file.

[Apache]

10.0.1.152 ansible_user=ec2-user ansible_ssh_private_key_file=PATH_OF_PEM_FILE

2) run the playbook

ansible-playbook -i /etc/ansible/hosts -b playbook.yml

------------------------------------------------------------------------
Directory Structure
.
├── playbook.yml
├── README.md
└── roles
    └── http
        ├── defaults
        │   └── main.yml
        ├── files
        │   ├── index.html
        │   └── web.conf
        ├── handlers
        │   └── main.yml
        ├── meta
        ├── tasks
        │   ├── main.yml
        │   ├── section_1.yml
        │   ├── section_2.yml
        │   └── section_3.yml
        ├── templates
        └── vars

9 directories, 10 files

