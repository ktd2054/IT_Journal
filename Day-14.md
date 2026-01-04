
# Windows 11 troubleshooting basics

## Common fixes

### Booting into Safe Mode

 - go to settings -> System -> Recovery -> Click Restart now in Advanced startup
    <img width="527" height="213" alt="image" src="https://github.com/user-attachments/assets/62f21168-b7b7-43e0-973f-9919a462b358" />
- Restart now and wait for options

- go to Troubleshoot -> Advanced Options
<img width="727" height="410" alt="image" src="https://github.com/user-attachments/assets/39aaf516-85c2-49cf-b69c-1a4b4298d94d" />
- Click on Startup Settings -> Restart

- Wait for options to be pressed

<img width="472" height="429" alt="image" src="https://github.com/user-attachments/assets/ecd43113-58f8-44a9-9b86-7a2bdff12a4e" />

- Click 4 for safe mode

<img width="688" height="257" alt="image" src="https://github.com/user-attachments/assets/fa93016b-9d45-4574-aada-b687773a040a" />

- Reboot the button.


### Resetting Windows


- go to settings -> system -> recovery -> reset this pc 

<img width="637" height="210" alt="image" src="https://github.com/user-attachments/assets/f67500b7-a87f-4bc0-bfd4-a9383953501f" />

- choose one of the options; i will remove everything

<img width="625" height="221" alt="image" src="https://github.com/user-attachments/assets/2b5aee92-f9f0-4e47-b6d2-15f4f79f1d08" />

- I chose local install -> click next 

<img width="496" height="282" alt="image" src="https://github.com/user-attachments/assets/41705383-f1d5-40db-8fb8-00dddcec942d" />

- click reset and after a while setup the device

### Restoring Windows 

- start -> controlpanel -> system and security -> system -> System Protection

<img width="693" height="422" alt="image" src="https://github.com/user-attachments/assets/775a76d1-f8fb-4c1e-b940-35e859dc68ef" />

- Both has protection off

- Select C drive -> configure -> turn on system protection

<img width="364" height="194" alt="image" src="https://github.com/user-attachments/assets/9e3cb1fc-4185-4374-8b9d-b57dec48c827" />

- to create a restore point click create

-  write description (such as Background) and click create 

-  change background color

-  lets use that restore point to take it back to normal

- go to control panel -> System and Security -> System -> System protection -> system restore -> click next choose the restore point we made

<img width="545" height="323" alt="image" src="https://github.com/user-attachments/assets/b5940641-d49e-495f-9173-37d5162c86d7" />

- click and finish -> yes and after reboot it is backed up

#### Troubleshooting tools

- Start -> Settings -> System -> Troubleshoot

How do they work?

- click on other troubleshooters

<img width="760" height="258" alt="image" src="https://github.com/user-attachments/assets/1e28a736-4700-4974-aa0c-089b5477b458" />

- look for troubleshooter that coresponds to the problems that we are having and click run


#### Cleaning hard disks

- Settings -> Sytsem -> Storage
  
<img width="1038" height="484" alt="image" src="https://github.com/user-attachments/assets/990f742e-ed58-48aa-ab13-b326905c1cea" />

- Temporary files are cleaned in order to free some spaces

- For automation, turn on Storage sense button

<img width="1022" height="262" alt="image" src="https://github.com/user-attachments/assets/22df5f59-dbc0-4e02-9280-f41c871cb938" />

- Click on the category to clean up such as in Temporray Files

#### Booting Problems

- use installation media and select repair your computer
  
<img width="610" height="457" alt="image" src="https://github.com/user-attachments/assets/c9e119c3-8da6-4a21-8ba5-9a741e32a11c" />

 - choose troubleshoot for startup problems

<img width="560" height="446" alt="image" src="https://github.com/user-attachments/assets/99575552-7c48-4f91-b03b-f8ce02f24eb2" />

- click on startup repair

<img width="438" height="265" alt="image" src="https://github.com/user-attachments/assets/a3c1d2c6-0660-4bf6-b65e-f7d5b96ed348" />

- it starts diagnosting pc


### Checking startup for malware

- run -> tskmgr
  
<img width="661" height="390" alt="image" src="https://github.com/user-attachments/assets/88da7736-9a60-4e20-8658-c1e4ff7bee55" />

- click startup icon on left (5th icon on left sidebar)

- we can see apps there

<img width="569" height="280" alt="image" src="https://github.com/user-attachments/assets/9aafd118-7676-44e4-adc5-c2ead070c904" />

- let's check 1 of the programs running

- select the acrobat program and clicking ... bar on right -> click open file location

<img width="792" height="243" alt="image" src="https://github.com/user-attachments/assets/12a4bb86-b49e-40c7-a38a-74621c3526ee" />

- check the files using internet if they are legitimate or not ; if not select the app and click disable on right; or if want to remove it completetly

- go to C:/ProgramData/Microsoft/Windows/Start Menu/Programs/Startup
- click and delete the file from the folder

<img width="960" height="215" alt="image" src="https://github.com/user-attachments/assets/1f4f4a7f-b69f-4f27-846b-d1d6d98230ff" />

### Troubleshooting the Applications

- Settings -> Apps -> Installed Apps -> Select the app that you want to fix
- Terminate or Repair or Reset or Uninstall and re-install ; depends on your choice

### Fixing an application compatiability problem 

- start -> all apps -> select -> right click -> more -> open file location -> select .exe file -> right click -> show more options -> troubleshoot compatiability

<img width="1013" height="603" alt="image" src="https://github.com/user-attachments/assets/61d1d388-75f5-4b8b-a0fa-6b82ff365019" />

 
