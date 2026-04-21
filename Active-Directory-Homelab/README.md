# Active Directory Home Lab (Oracle VirtualBox)

## Project Summary
Built a virtualized Active Directory environment using Oracle VirtualBox. Configured a Windows Server 2025 Domain Controller and a Windows 11 client machine. Created organizational units, users, and groups, and successfully joined the client machine to the domain using domain credentials.

## Environment / Tech Stack
- Oracle VirtualBox
- Windows Server 2025 (Domain Controller)
- Windows 11 (Client Machine)
- Active Directory Domain Services (AD DS)
- DNS

## Lab Setup
- Created two virtual machines:
  - Windows Server 2025 (Domain Controller)
  - Windows 11 (Client)
- Configured networking to allow communication between machines
- Promoted Windows Server to Domain Controller
- Installed and configured Active Directory Domain Services

## Active Directory Configuration
- Created Organizational Units (OUs)
- Created domain users
- Created security groups
- Added users to groups
- Assigned Domain Admin privileges to selected users

## Domain Join Process
- Configured Windows 11 client DNS to point to Domain Controller
- Used domain credentials created in Active Directory
- Successfully joined Windows 11 machine to the domain

## Screenshots

![VM Setup](screenshots/vm_setup.png)
![AD Users](screenshots/ad_users.png)
![OUs](screenshots/ous.png)
![Groups](screenshots/groups.png)
![Domain Join](screenshots/domain_join.png)
![Success](screenshots/domain_success.png)
