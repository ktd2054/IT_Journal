# Project 1: Microsoft 365 Security Baseline Hardening & User Access Management

## Summary

This project demonstrates a lifecycle of user identity and access management in microsoft 365 from an IT support prespective. It includes creating users, onboarding, configuring security, troubleshooting login issues, managing shared resources and analysing the logs. 

## Objectives

- To handle enrollment and exit
- Manage users, groups and shared mailboxes
- Troubleshoot sign-in/MFA issues
- Understand password and authentication security
- Perform core admin tasks required at the IT support level
- Document the workflows

## Tools Used

- M365 Admin Center
- Azure AD/ Entra ID
- Microsoft Defender Admin
- M365 Compliance center
- Exchanage Admin Center

## LabWork 

### Lab 1 - User Onboarding Workflow

#### Step 1: Creating user accounts

Go to Admin center -> users -> Active users -> Add user

Users Created Successfully and Assigned M365 Licenses

<img width="979" height="398" alt="image" src="https://github.com/user-attachments/assets/55454b17-d4d2-433f-ab7d-a658973c0e4d" />

#### Step 2: Adding users to security/distribution groups and Creating shared mailboxes

Go to Groups -> Active Groups -> Add Group

- Created groups for each department and assigned team members. 

<img width="923" height="463" alt="image" src="https://github.com/user-attachments/assets/1c3bd012-7efa-41e8-bd82-21b46284545e" />

- Created Shared Mailboxes
  
<img width="916" height="642" alt="image" src="https://github.com/user-attachments/assets/9f01d7d9-8337-4821-adc7-96c46090348c" />

#### Step 3: Enabling and Reviewing Security Configuration

Go to Active users -> Multi-factor authentication -> New Policy -> Select users or agents -> check select users and groups

- selecting users by clicking the box and press the select button
  Name: Users MFA

Grant -> click on 0 controls selected -> grant access -> check require multifactor authentication

Next, Sessions -> click sign-in frequency -> select periodic authentication -> enter 90 and select days from the select box

<img width="676" height="615" alt="image" src="https://github.com/user-attachments/assets/ed558c5a-6bdc-438b-a54a-0b60c4aefa50" />

Successfully created users MFA for users.

### Lab 2

#### Log Analysis

- Audit Logs

Go to Entra -> Roles & Admins -> Click Audit Logs

analyse the logs 

- Sign-in Logs

Go to Enterprise apps  -> click on Sign-in Logs

Monitor the logs.

## References

- https://learn.microsoft.com/en-us/microsoft-365/admin/?view=o365-worldwide
  
- https://learn.microsoft.com/en-us/microsoft-365/admin/add-users/add-users?view=o365-worldwide
  
- https://learn.microsoft.com/en-us/entra/identity/authentication/tutorial-enable-azure-mfa




