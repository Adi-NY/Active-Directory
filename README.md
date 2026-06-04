# Active Directory , User and Role Management
## Real-World Identity and Access Management Lab

## Overview
Built a fully functional Active Directory domain environment
using VirtualBox and Windows Server 2025 to develop hands-on
experience with enterprise identity and access management.
This lab simulates a real-world organizational IT environment
including domain setup, user and group management, GPO
configuration, remote access, and client machine integration.

## Environment
| Component | Details |
|-----------|---------|
| Hypervisor | VirtualBox |
| Server OS | Windows Server 2025 |
| Client OS | Windows 11 |
| Domain | adiit.lab |
| Lab Type | On-Premise Active Directory |

## Skills Demonstrated
- Organizational Unit (OU) design and hierarchy
- User account creation and lifecycle management
- Security group creation and role-based access control (RBAC)
- Group Policy Object (GPO) configuration
- Account lockout policy enforcement
- Password policy configuration
- Role delegation with least privilege principles
- Remote Desktop Protocol (RDP) access management
- Client machine domain join and authentication
- SYSVOL logon script configuration
- Account lockout identification and recovery
- Temporary password assignment and forced reset

## Real World Application
| Lab Task | Real World Scenario |
|----------|-------------------|
| OU Creation | Organizing staff by department for targeted policy application |
| User Account Creation | New employee onboarding, IT provisioning access on Day 1 |
| Security Group Assignment | Ensuring staff only access systems relevant to their role |
| GPO - Password Policy | Enforcing organization-wide password security standards |
| GPO - Account Lockout | Protecting against brute force login attempts |
| Role Delegation | Granting helpdesk staff limited admin rights without full domain admin |
| Account Lockout Recovery | Staff locked out, common helpdesk scenario |
| Temporary Password | Secure credential handoff during password reset procedure |
| Domain Join | Setting up a new workstation for a new hire |
| SYSVOL Logon Script | Automating drive mapping so staff have correct folders on login |
| RDP Configuration | Enabling IT staff to remotely support users without being onsite |
| Login Restriction | Preventing staff from logging in outside their shift hours |

## Notable Scenario, Duplicate Group Assignment
During the lab a duplicate group assignment error was encountered
and documented. This real-world troubleshooting scenario
demonstrates the importance of naming conventions in an enterprise
AD environments, a lesson applied by implementing standardized
group naming before continuing.

## Lab Walkthrough

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

## Key Takeaways
- OU structure is the foundation of effective GPO application,
  policies applied at the wrong level affect unintended users
- Least privilege through role delegation is more secure than
  granting full domain admin rights for limited administrative tasks
- Naming conventions must be established before group creation,
  duplicate names cause assignment failures in production environments
- SYSVOL logon scripts significantly reduce manual onboarding
  steps by automating drive mapping on user login
- Account lockout policies must balance security with usability,
  too aggressive and you create unnecessary helpdesk tickets

## Connect
- LinkedIn: linkedin.com/in/nuhabkhan
- Portfolio: github.com/Adi-NY/it-portfolio
- Email: adiibnekhann@gmail.com
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
