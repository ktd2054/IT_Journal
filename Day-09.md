# Networking

Networking is the practice of connecting two or more computing devices together so they can exchange information. 
This is done using a combination of:
- Hardware (routers, switches, cables)
- Software (operating systems, firewalls)
- Protocols (rules like TCP/IP)

The main objective of networking is resource sharing. This means allowing multiple devices (like computers, printers, and servers) 
to communicate with each other to share data, services (like internet access), and hardware (like a shared printer).

### Summary 

#### What I'm Doing in This Networking Section?

In this section, I'm learning the practical, hands-on skills for a Level 1 (L1) network support job.
I'm moving beyond just knowing what terms like TCP/IP, DNS, DHCP, and Routers mean. 
I'm using a network simulator to build a virtual small office network from scratch to see how all these services work together.
The main goal is to practice real-world troubleshooting. I'm intentionally breaking the network in different ways 
and then using standard IT support tools to diagnose the problem and fix it, just like in a real-world scenario.


### Lab 1: Creating a small office network

Tools: Router(2911), Switch(2960), PC0, PC1,  

a) bulding a structure

b) configurations

Router configuration

- click the router
- go to command line tab
- write commands to configure IP address and subnet mask sequentially
  enable
  
  configure terminal
  
  interface GigabitEthernet0/0
  
  ip address 192.168.1.1 255.255.255.0
  
  no shutdown
  
  exit


<img width="401" height="496" alt="image" src="https://github.com/user-attachments/assets/847695a7-11ea-4a95-a0b1-349316c70fca" />

This screenshot shows a fully converged network. The green triangles on all the connection points mean the links are active and ready to pass data. The switch has finished its startup process (STP), and the router's interface is up. The router's DHCP service is configured correctly, and the PCs successfully got their IP addresses.
