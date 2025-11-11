# Setting up the DNS and DHCP

Summary:
Set up a Windows Server virtual machine in VirtualBox and configured it as a Domain Controller for the internal domain cybersec.com. The server also provides DNS for name resolution and DHCP to automatically assign IP addresses to client systems. A Windows 10 machine will be joined to the domain for authentication testing and user management practice.

Objectives:

- Install and configure Windows Server as a Domain Controller

- Set up DNS for internal hostname resolution

- Configure DHCP to automatically assign IP addresses

- Create and manage domain users and groups

- Join a client computer to the cybersec.com domain

# Installation of Windows Server 2019

<img width="818" height="564" alt="image" src="https://github.com/user-attachments/assets/f8107d0f-25da-42ee-9a7c-d2f1c6411fea" />

## Setup and install Domain Controller and DNS Server

<img width="713" height="507" alt="image" src="https://github.com/user-attachments/assets/57e8534c-3a64-4814-80bc-1318dd91d8a9" />

a) Open Sever Manager 

b) Go to local server - computer name - change and set name

c) on the top click Manage - Add Roles and Features

d) click until server roles

e) check the box Active Directory Domain Services 

f) click Add Features - next - install - promote this server to a domain controller

g) choose add a new forest

h) set domain name and password

i) click next and install

<img width="719" height="467" alt="image" src="https://github.com/user-attachments/assets/f107fc6b-4ad6-4039-9f5a-35a313fdd8d8" />

## Configurating DHCP

Before configuring the DHCP, we have to change network in virtualbox settings. Go to VirtualBox and click the os name and go to settings. 

Set Network Adapter1 to NAT and Adapter2 to Host-only Network. After setting up the network, run ipconfig command in command prompt inside VBox Windows Server. Check if the ip address for ethernet and ethernet2. When I checked my IP it was different from each other
and also the subnet mask as Windows couldnot find any DHCP server or assigned network.

<img width="300" height="134" alt="Screenshot 2025-11-12 074952" src="https://github.com/user-attachments/assets/4d04c816-5047-41b5-ad40-3f4e037b30b1" />

We need to assign the static IP to Ethernet2. 

- go to control panel -> network and internet -> network and sharing center -> change adapter settings

- click ethernet2 -> properties -> select IPv4 -> properties
  
- select use the following IP addresses
  
- assign IP address and subnet mask
  
- use same IP to preferred DNS server
  
- click ok and close

Go to cmd and check the IP address using ipconfig command. Voilà, 

<img width="280" height="129" alt="Screenshot 2025-11-12 080010" src="https://github.com/user-attachments/assets/8f414c58-d59c-4a89-9bc3-fb84b2062388" />

#### Install and Configure DHCP

- Server Mananager -> Manage -> Add Roles and Features
- Click Next till Server Roles -> Tick DHCP Server
- Click Add Features -> Next -> Install
- After installing, click the flag on top
- Go to complete the DHCP configuration
- click next -> commit and close

go to Tools and we will see DHCP

<img width="577" height="411" alt="image" src="https://github.com/user-attachments/assets/8c8e69af-cb21-493e-b345-45c5af21d80f" />

- Click on DHCP,
<img width="1182" height="363" alt="image" src="https://github.com/user-attachments/assets/9cb693d7-d679-4ed3-8bbd-e43965c7f597" />

- Select IPv4 and right-click
  
- Open New Scope and setup wizard will open
  
- Giving the scope a name "OfficeLAN"

- setting up starting IP and ending IP

- click next and skip add exclusions and delay wizard

- click next and select yes on configuation part

- set router ip and next till finish

Our DHCP server is live and now any client in Host-only network will receive IP 192.168.xx.x, gateway 192.168.xx.x and dns 192.168.xx.x

Next steps is to add a Windows 10 Client.

- Install Windows and run ipconfig command

<img width="223" height="87" alt="Screenshot 2025-11-12 094745" src="https://github.com/user-attachments/assets/c9342c94-e88e-4ab7-9731-a5612a6ea89d" />

it's connected to our server.
