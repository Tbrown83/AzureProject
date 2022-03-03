# AzureProject
Azure JumpBox,VMs and Elk Sever operation
The files in this repository were used to configure the network depicted below.

(diagram.png)

These files have been tested and used to generate a live ELK deployment on Azure. They can be used to either recreate the entire deployment pictured above. Alternatively, select portions of the playbook file may be used to install only certain pieces of it, such as Filebeat.

filebeat-playbook.yml

This document contains the following details:

Description of the Topologu
Access Policies
ELK Configuration
Beats in Use
Machines Being Monitored
How to Use the Ansible Build
Description of the Topology

The main purpose of this network is to expose a load-balanced and monitored instance of DVWA, the D*mn Vulnerable Web Application.

Load balancing ensures that the application will be highly efficient in distributing incoming network traffic, in addition to restricting unneccesary access to the network. Load Balancers help to protect the servers against DDoS attacks. Jumpbox acts as gateway router which allows security professionals to implement strong access controls on a single machine rather than on every individual virtual machine, which reduces the attack surface.

Integrating an ELK server allows users to easily monitor the vulnerable VMs for changes to the logs and system files.

Filebeat collects data about the file system.
Metricbeat records machine metrics._
The configuration details of each machine may be found below. Note: Use the Markdown Table Generator to add/remove values from the table.

Name	Function	IP Address	Operating System
Jump Box	Gateway	10.0.0.4	Linux
Web-1	Virtual Machine	10.0.0.7	Linux
Web-2	Virtual Machine	10.0.0.9	Linux
ELK	Virtual Machine	10.1.0.5	Linux
