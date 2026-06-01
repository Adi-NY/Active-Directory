<h1>Active Directory - User and role management w/ Real World Scenarios </h1>


<h2>Description</h2>
Built a fully functional Active Directory domain environment 
using VirtualBox and Windows Server 2025 to develop hands-on 
experience with enterprise identity and access management. 
This lab simulates a real-world organizational IT environment 
including domain setup, user and group management, GPO 
configuration, remote access, and client machine integration.
<br />

<h2>Environments Used </h2>

| Component | Details |
|-----------|---------|
| Server OS | Windows Server 2025 |
| Client OS | Windows 11 |
| Domain | adiit.lab |
| Lab Type | Local Active Directory |

<h2>Program walk-through:</h2>

<p align="center">
Creating Organizational Units (OUs): <br/>
<img src="https://i.imgur.com/S5W8ujB.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />
Creating User Accounts:  <br/>
<img src="https://i.imgur.com/IitwZ4Z.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />
Updating User Information: <br/>
<img src="https://i.imgur.com/3GI8Xpk.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />
Creating Group/Roles:  <br/>
<img src="https://i.imgur.com/2a6eui7.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />
Assigning Security Permissions to Groups:  <br/>
<img src="https://i.imgur.com/IhpYJ7P.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />
Assigning Group to Created Users:  <br/>
<img src="https://i.imgur.com/WV2L9Qc.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />
Assigning Group to Created Users (Duplicate Scenario):  <br/>
<img src="https://i.imgur.com/b2lMqPY.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />
Assigning Login Restriction Time to Users:  <br/>
<img src="https://i.imgur.com/Xz2PDEC.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />
Configuring Account Lockout Policy to Group Policy (GPO):  <br/>
<img src="https://i.imgur.com/LGZQjrG.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />
Configuring Password Policy:  <br/>
<img src="https://i.imgur.com/bgQjqFh.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />
Configuring Role Delegation:  <br/>
<img src="https://i.imgur.com/DjYhCwy.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />
Connecting Client PC to Domain Controller's VNET:  <br/>
<img src="https://i.imgur.com/bbgmk4L.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />
Adding Client PC to Remote Desktop User (since we are connecting through Remote Desktop Connection):  <br/>
<img src="https://i.imgur.com/hluBEna.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />
Connecting Client PC to Domain:  <br/>
<img src="https://i.imgur.com/6MpwQZu.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />
Domain Connection Successful:  <br/>
<img src="https://i.imgur.com/HrA4Eue.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />
Client Domain Overview:  <br/>
<img src="https://i.imgur.com/YD7YQKs.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />
Logging into Client PC as Domain User:  <br/>
<img src="https://i.imgur.com/wILk1mx.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />
Test Account Lockout Scenario:  <br/>
<img src="https://i.imgur.com/7v6rVTw.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />
Active Directory showcasing locked account:  <br/>
<img src="https://i.imgur.com/TpCMNmI.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />
Unlocking User Account:  <br/>
<img src="https://i.imgur.com/9ACyYCA.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />
Assigning Temporary Password to Client:  <br/>
<img src="https://i.imgur.com/XUf7u66.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
<br />
<br />  
Configuring SYSVOL for User account:  <br/>
<img src="https://i.imgur.com/J4bEM8L.png" height="80%" width="80%" alt="Active Directory Walkthrough"/>
</p>


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
