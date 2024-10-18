Ansible Role
=========

This repository contains two Ansible roles combined into one. The roles are organized as follows:

Tasks (Jenkins Installation):

Located in tasks/main.yml
This role is responsible for installing Jenkins on your system.
Handlers/main.yml 
This role is responsible for installing docker on your system.

How to Run the Playbooks
To use these roles, follow the commands below:

Install Jenkins:
Copy code

ansible-playbook -i tests/inventory tasks/main.yml

Install Docker:
Copy code

ansible-playbook -i tests/inventory handlers/main.yml

Configuration
Before running the playbooks, please ensure to make the following changes:

Update the Inventory File:

Navigate to tests/inventory.
Change the IP address to your personal address.
Modify Host Names:

In the inventory file, change the name [workstation] to match your environment.
Update the host names in both tasks/main.yml and handlers/main.yml as necessary.
