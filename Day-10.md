# Setting up the DNS and DHCP

Summary

Objectives


- Installation of Windows Server 2019

<img width="1018" height="764" alt="image" src="https://github.com/user-attachments/assets/f8107d0f-25da-42ee-9a7c-d2f1c6411fea" />

## Setup and install Domain Controller and DNS Server

<img width="1013" height="707" alt="image" src="https://github.com/user-attachments/assets/57e8534c-3a64-4814-80bc-1318dd91d8a9" />

a) Open Sever Manager 
b) Go to local server - computer name - change and set name
c) on the top click Manage - Add Roles and Features
d) click until server roles
e) check the box Active Directory Domain Services 
f) click Add Features - next - install - promote this server to a domain controller
g) choose add a new forest
h) set domain name and password
i) click next and install

<img width="1019" height="767" alt="image" src="https://github.com/user-attachments/assets/f107fc6b-4ad6-4039-9f5a-35a313fdd8d8" />

- Configurating DHCP

Before configuring the DHCP, we have to change network in virtualbox settings. Go to VirtualBox and click the os name and go to settings. 
Set Network Adapter1 to NAT and Adapter2 to Host-only Network. After setting up the network, run ipconfig command in command prompt inside
VBox Windows Server.






