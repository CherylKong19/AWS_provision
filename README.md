# Automate AWS_provision
This repository contains all main files to automate AWS provision.

### Pre-requisite
1. Ansible is installed
2. Configure basic localhost information and aws info in ansible inventory

### Before running the code
1. Change all needed information like vpc, subnet info
2. Set default variables in each folder
3. Make sure aws_zone is the same you set in the code

### To create RDS instance
1. Change all "rds_database" to True
2. Run command `ansible-playbook --tags provision`

### To create databases in ec2
1. Change all "rds_database" to False
2. Run command `ansible-playbook --tags provision`

### To get information for ec2 and databases
1. Run command `ansible-playbook --tags info`

### To destroy all created instances 
1. Run command `ansible-playbook --tags destroy`
