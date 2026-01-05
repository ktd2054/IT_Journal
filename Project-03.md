# Intune Device Enrollment and Policy Management

## Objectives

- A Microsoft 365 tenant with test users
- A Windows device enrolled into Intune
- Groups for targeting policies
- Compliance policy (pass/fail rules)
- Configuration profile (settings pushed to device)
- Documentation

## Setup Checklist

- M365 account and license
- Intune admin center

## Creating test users

- I have already created test users in previous task [Project-1: Click Here](Project-01.md) and has assigned them to distinct
departments such as Sales, Finance, IT and HR.

<img width="1656" height="594" alt="image" src="https://github.com/user-attachments/assets/61f7df90-773d-429d-94b5-cc35c41921f6" />

## Creating Security Groups (SG) for Intune

- As I mentioned I have already created departmental groups

<img width="1836" height="787" alt="image" src="https://github.com/user-attachments/assets/37b21dcd-3b93-4ad0-bb59-f21906565a25" />

- But now I will create security groups for intune because intune policies works with security groups.

- Navigating to Entra ID -> Groups -> New Groups -> filled the info and selected 3 members

<img width="820" height="607" alt="image" src="https://github.com/user-attachments/assets/65f68093-65dc-4498-a564-69c0c2e0ea93" />

- Now, creating security group for Devices -> fill the form and left member field unselected for next time

<img width="752" height="665" alt="image" src="https://github.com/user-attachments/assets/f99a4559-884e-401a-8b49-c454170e538a" />

## Enrolling a windows 10/11 device into intune 

- Using Windows 11 Vm for signing in.

<img width="572" height="435" alt="image" src="https://github.com/user-attachments/assets/df2730ab-b406-437e-8037-939d407ea786" />

- using one of the accounts to login and after logging in successfully it only shows in Entra

<img width="1541" height="412" alt="image" src="https://github.com/user-attachments/assets/836bb978-2fe1-4d3d-894f-3c25f1244270" />

- And did not show any devices on Intune

- I searched for this error and got the fix (https://learn.microsoft.com/en-us/intune/intune-service/user-help/enroll-windows-10-device)
- downloaded company portal app using microsoft store
- now setting up the app using same member account
- connecting that account with work
- registering the device

<img width="913" height="689" alt="image" src="https://github.com/user-attachments/assets/7a29078a-cb95-460c-bbd5-ae1763b9c5da" />

- yes yes yes, it showed

<img width="1893" height="716" alt="image" src="https://github.com/user-attachments/assets/22a3e5c4-3bbd-41b3-adc1-0c06a7c4f134" />

## Creating a Windows Compliance Policy

- Go to Devices -> Compliances -> Policies -> create policy -> platform windows 10 or later -> Windwos 10/11 compliance policy -> create
- Fill the details
<img width="861" height="532" alt="image" src="https://github.com/user-attachments/assets/e4b42729-e5bf-40ba-91e9-b022d815af5f" />
- selecting passwords under system security adn configuring the security

<img width="768" height="426" alt="image" src="https://github.com/user-attachments/assets/6292e130-c804-4353-875c-8b6e6ed04853" />

- click create 
<img width="763" height="757" alt="image" src="https://github.com/user-attachments/assets/31d0763a-6a4b-40cc-8f73-c5f7e9d5dff6" />

### Why did we set compliance?

==> Because it checks whether a device meets the security standards or not.

## Windwos Configuration Profile

- To ensure that a compliance policy always warns users to meet the compliance i.e. Enforces security settings for corporate Windows devices

-  An example would be What if user turns of firewall:

-  go to devices -> configuration -> create -> Platform: Windows 10 and later -> Profile type: Settings catalog -> Click Create

<img width="823" height="406" alt="image" src="https://github.com/user-attachments/assets/6edfc0c4-3971-4add-81e6-e5f6c7c50c81" />

- I will search Defender and select allow antimalware service to remain running always

- What that does ? ==> protect against malware trying to disable protection

- save


