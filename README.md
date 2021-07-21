#Terraform Modules to provision a VM in Azure
 - resourcegroup - creating resourcegroup
 - networking - creating azure virtual network and required subnet
 - securitygroup - creating network security group to allow https 
 - compute - creating network interfaces and virtual machines
  
 Azure Resources - RG, Vnet, Subnet, NSG, NIC, VM
	
#Manual Deployment / Provision a VM - 
1. checkout repo in a linux VM
2. make sure terraform installed 
3. execute below commands from Cloud-Domain-Assesment directory
 - terraform init
 - terraform plan
 - terraform validate
 - terraform apply

#Ansible playbook to install Tomcat web server 
 - tomcat-node - update IP address/host name 
 - install-tomcat.yml - Ansible playbook to install Tomcat server

#Install Tomcat - 
1. checkout repo in a linux VM
2. Change directory to Cloud-Domain-Assesment/ansible then execute playbook
   - ansible-playbook -i tomcat-node install-tomcat.yml

#Deploy application packege war/ear into tomcat server  
1. added this task in ADO pipeline 


-------------------------------------------------------------------------------
Multi stage ADO pipeline to 
- Provision a VM in Azure cloud
- Install tomcat into VM
- Build Application - into a war file
- Deploy a war file into Tomcat server 
 


