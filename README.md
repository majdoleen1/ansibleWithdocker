# ansibleWithdocker
# ansible
# Project Overiew
This project Deploys a weight-tracker app image from a Control Node VM into Scale Set VMs which perform as agents over 2 environments: Staging and Production.

the infrastructure was created in Terraform and can be seen here:
https://github.com/majdoleen1/week5


## Main Components:
* 2x Load Balancer
* 2x VM + 1 scale set VM with 3 instances.
* 2x Managed Flexible PostgresQL DB Server

All the files can be Cloned, Credential File excluded.

## installation Guide:
 1. Clone The project
 2. in the control node,place the main.yml file in the vars directory
 3. in folder's root, press ansible-playbook -i "inventory/<Chosen Enviornment>" --ask-become-pass main.yml
 4. enter the agents computer password.
 
 as a result, the script will be deplyed to the agents.
