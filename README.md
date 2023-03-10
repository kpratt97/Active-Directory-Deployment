
<h1>Active Directory Deployment</h1>

 ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo)

<h2>Description</h2>
Active Directory is a database and set of services that connect users with the network resources they need to get their work done. The database (or directory) contains critical information about your environment, including what users and computers there are and who's allowed to do what.
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell Ise</b> 
- <b>Server Manager</b>
- <b>Microsoft Azure</b>
<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)
- <b>Remote Desktop</b>

<h2>Program walk-through:</h2>

<p align="center">
Step 1: Creating the Domain Controller and Client through Microsoft Azure <br/>
<br />
<br />


https://user-images.githubusercontent.com/119460677/213619351-5dde2022-8b5a-4b68-850d-fec003823826.mp4




<br />
<br />
<p align="center">
Step 2: In Azure we will set the Domain Controller’s NIC Private IP address to be static
<br/>
 
https://user-images.githubusercontent.com/119460677/213609792-7a9cd55c-b7e6-4031-8237-79514d4d58eb.mp4

<br />
<br />
<p align="center">
Step 3: Login to the Domain Controller remote desktop and enable ICMPv4 Protocols through Windows Firewall: <br/>
<br />
 
https://user-images.githubusercontent.com/119460677/213612294-610c95ef-d380-4f13-b2c8-b88996f2308a.mp4

<br />
<br />
<br />
<p align="center">
Step 4: While in DC-1 I will install Active Directory Domain Services  
<br/>
<br />
 
https://user-images.githubusercontent.com/119460677/213621848-956ab6bb-2e68-445b-a203-094e8e749160.mp4

<br />
<br />
<p align="center">
Step 5: Create a new forest as mydomain.com 
<br />
<br />
<img src="https://i.imgur.com/JusQXiY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<br />
Step 6: Creating an Organizational Unit in AD Users and Computers (_EMPLOYEES_ AND _ADMINS_)
<br />
<br />
 
https://user-images.githubusercontent.com/119460677/213623591-ce98c861-3f94-44cd-95ca-37e35889df54.mp4


<br />
<br />
 <p align="center">
Step 7: Creating a new employee named Luffy Monkey, creating a password and adding Luffy to the "Domain Admins"  <br/>
</p>


https://user-images.githubusercontent.com/119460677/213626070-d3ef4de0-7696-4940-8257-692d417dd1fb.mp4


<br />
<br />






Step 8: In Azure Virtual Machines I'll be joining Client 1 to my domain. Setting client 1's DNS settings to DC's private IP address  <br/>


https://user-images.githubusercontent.com/119460677/213627540-ebfa1117-f602-40eb-9c1f-0fe5acb08e2d.mp4


</p>
<br />
<br />
Observe the wiped disk:  <br/>


https://user-images.githubusercontent.com/119460677/213628327-a2a802f5-d735-469e-af4e-60cdeda8b895.mp4


</p>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/JusQXiY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
