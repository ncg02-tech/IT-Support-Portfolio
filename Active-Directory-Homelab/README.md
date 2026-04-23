# Active Directory Home Lab (Oracle VirtualBox)

## Overview
Built and configured a virtualized enterprise-style Active Directory environment using Oracle VirtualBox. Deployed a Windows Server 2025 Domain Controller and a Windows 11 client, implemented domain services, and validated authentication through a successful domain join.

---

## Environment / Tech Stack
- Oracle VirtualBox (Virtualization)
- Windows Server 2025 (Domain Controller)
- Windows 11 (Client Machine)
- Active Directory Domain Services (AD DS)
- DNS
- TCP/IP Networking

---

## Lab Architecture
- Deployed two virtual machines:
  - Domain Controller (Windows Server 2025)
  - Client Workstation (Windows 11)
- Configured internal networking for VM-to-VM communication
- Assigned static IP address to Domain Controller
- Configured client machine to use Domain Controller as primary DNS

---

## Server Configuration
- Installed Active Directory Domain Services (AD DS)
- Promoted server to Domain Controller
- Configured domain environment
- Verified hostname and remote management settings
- Installed and validated required server roles and features

---

## Active Directory Management
- Created Organizational Units (OUs) to simulate enterprise structure
- Created multiple domain user accounts
- Created and configured security groups
- Added users to groups to manage access control
- Assigned Domain Admin privileges to designated user accounts

---

## Client Configuration
- Installed and updated Windows 11 client
- Configured network adapter settings
- Verified DNS resolution to Domain Controller
- Ensured connectivity between client and server

---

## Domain Join Process
- Configured client machine DNS to point to Domain Controller
- Used domain credentials created in Active Directory
- Successfully joined Windows 11 machine to the domain
- Verified domain authentication by logging in with domain user
- Confirmed domain connectivity and access permissions

---

## Key Skills Demonstrated
- Active Directory Administration
- User and Group Management
- Domain Controller Deployment
- DNS Configuration
- Network Configuration (TCP/IP)
- Virtualization (Oracle VirtualBox)
- Windows Server Management
- Endpoint Domain Integration

---

## Key Takeaways
- Proper DNS configuration is critical for domain functionality and authentication
- Active Directory structure relies on organized OUs, users, and group-based permissions
- Domain Controllers must be correctly configured before client integration
- Step-by-step validation is essential when deploying enterprise environments

## Screenshots

### 1. Downloading Installation Files
![Windows 11 ISO](screenshots/01_windows_11_iso.png)
![Windows Server 2025 ISO](screenshots/02_windows_server_2025_iso.png)
![Oracle VirtualBox Download](screenshots/03_oracle_virtualbox_download.png)

### 2. Creating the Windows Server Virtual Machine
![New Windows Server VM 1](screenshots/04_new_windows_server_vm_1.png)
![New Windows Server VM 2](screenshots/05_new_windows_server_vm_2.png)
![New Windows Server VM 3](screenshots/06_new_windows_server_vm_3.png)
![New Windows Server VM 3](screenshots/06.1_new_windows_server_vm_3.png)
![Windows Server Setup](screenshots/07_windows_server_setup.png)
![Server Manager](screenshots/13_server_manager.png)

### 3. Creating the Windows 11 Virtual Machine
![New Windows 11 VM](screenshots/08_new_windows_11_vm.png)
![New Windows 11 VM 1](screenshots/09_new_windows_11_vm_1.png)
![New Windows 11 VM 2](screenshots/10_new_windows_11_vm_2.png)
![New Windows 11 VM 3](screenshots/11_new_windows_11_vm_3.png)
![Windows 11 Home Page](screenshots/12_windows_11_home_page.png)

### 4. Initial Server Setup
![Server to Settings](screenshots/14.1_server_manager_to_settings.png)
![Server Download and Install Updates](screenshots/14_server_download_install_updates.png)
![Server Updates Completed](screenshots/18_server_updates_completed.png)
![Enable Remote Management](screenshots/17_enable_remote_management.png)

### 5. Initial Server Setup
![Windows 11 Home Page to Settings](screenshots/15.1_windows_11_home_to_settings.png)
![Windows 11 Download and Install Updates](screenshots/15_windows_11_download_install_updates.png)
![Windows 11 Updates Completed](screenshots/19_windows_11_updates_completed.png)

### 6. Installing Active Directory Domain Services
![Add Roles and Features Wizard 1](screenshots/20_add_roles_features_1.png)
![Add Roles and Features Wizard 2](screenshots/21_add_roles_features_2.png)
![Add Roles and Features Wizard 3](screenshots/22_add_roles_features_3.png)
![Add Roles and Features Wizard 4](screenshots/23_add_roles_features_4.png)
![Add Roles and Features Wizard 5](screenshots/24_add_roles_features_5.png)
![Add Roles and Features Wizard 6](screenshots/25_add_roles_features_6.png)
![Add Roles and Features Wizard 7](screenshots/26_add_roles_features_7.png)
![Add Roles and Features Wizard 8](screenshots/27_add_roles_features_8.png)
![Add Roles and Features Wizard 8](screenshots/27.1_add_roles_features_8.png)
![Add Roles and Features Wizard 8](screenshots/27.2_add_roles_features_8.png)
![Add Roles and Features Wizard 8](screenshots/27.3_add_roles_features_8.png)
![Add Roles and Features Wizard 8](screenshots/27.4_add_roles_features_8.png)

### 7. Server Network Configuration
![Changed Windows Server Network Settings](screenshots/28_changed_windows_server_network.png)
![Check Server IP Address](screenshots/30_server_ip_address.png)
![Set Static IP Address on Server](screenshots/30.1_server_static_ip.png)

### 8. Windows 11 Network Configuration
![Changed Windows 11 VM Network Settings](screenshots/29_changed_windows_11_network.png)
![Windows 11 IP Settings](screenshots/29.1_windows_11_ip_settings.png)
![Assign DNS Server to Windows 11 VM](screenshots/30.2_windows_assign_dns.png)

### 9. Active Directory Organizational Structure
![Creating Organizational Unit](screenshots/31_creating_organizational_unit.png)
![Organizational Units](screenshots/32_organizational_units.png)

### 10. Creating Domain Users
![New User](screenshots/33_new_user.png)
![New User 1](screenshots/34_new_user_1.png)
![New User 2](screenshots/35_new_user_2.png)

### 11. Assigning Group Permissions
![Carl Smith Add to Domain Admins 1](screenshots/36_carl_smith_domain_admins_1.png)
![Carl Smith Add to Domain Admins 2](screenshots/37_carl_smith_domain_admins_2.png)
![Carl Smith Add to Domain Admins 3](screenshots/38_carl_smith_domain_admins_3.png)

### 12. Joining the Windows 11 Client to the Domain
![Join Domain 1](screenshots/40_join_domain_1.png)
![Join Domain 2](screenshots/41_join_domain_2.png)
![Join Domain 3](screenshots/42_join_domain_3.png)

### 13. Authentication and Domain Verification
![Authenticate with Domain Credentials](screenshots/43_authenticate_domain_credentials.png)
![Now Connected to Domain](screenshots/44_now_connected_to_domain.png)
![Join Domain as Domain Admin](screenshots/45_join_domain_as_domain_admin.png)
![Proof of Domain User Logged In](screenshots/46_domain_user_logged_in.png)
