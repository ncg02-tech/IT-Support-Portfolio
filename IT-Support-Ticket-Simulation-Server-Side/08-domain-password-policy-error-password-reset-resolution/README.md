# Domain Password Policy Error – Password Reset and Policy Correction

## Summary
Authentication issues caused by misconfigured user account password policy settings in Active Directory.

## User
Anthony Walker

## Department
Marketing

## Issue
User not prompted to change password at first logon and unable to manage credentials properly due to incorrect account configuration.

---

## Troubleshooting
- Reviewed password-related authentication issues  
- Accessed **Active Directory Users and Computers (ADUC)**  
- Located user account within appropriate OU  
- Reviewed **account policy settings**  
- Identified misconfiguration:
  - “User must change password at next logon” disabled  
  - “User cannot change password” enabled  
- Determined root cause as **incorrect password policy configuration**  
- Updated account settings to allow password management  
- Initiated password reset  

---

## Resolution
- Enabled enforced password change at next logon  
- Restored user ability to manage credentials  
- Reset password to temporary value  
- Verified successful authentication and password update  

---

## Screenshots

### 1. Ticket (Spiceworks)
![Ticket](screenshots/0.png)

### 2. Reported Issue
![Issue](screenshots/0a.png)

### 3. Troubleshooting Steps
![Troubleshooting](screenshots/1.png)
![Troubleshooting](screenshots/2.png)
![Troubleshooting](screenshots/3.png)
![Troubleshooting](screenshots/4.png)
![Troubleshooting](screenshots/5.png)
![Troubleshooting](screenshots/6.png)
![Troubleshooting](screenshots/7.png)
![Troubleshooting](screenshots/8.png)
![Troubleshooting](screenshots/9.png)
![Troubleshooting](screenshots/10.png)
![Troubleshooting](screenshots/11.png)
![Troubleshooting](screenshots/12.png)

### 4. Issue Resolved (Working State)
![Resolved](screenshots/13.png)
![Resolved](screenshots/14.png)
![Resolved](screenshots/15.png)
![Resolved](screenshots/16.png)
![Resolved](screenshots/17.png)
![Resolved](screenshots/18.png)
![Resolved](screenshots/19.png)
![Resolved](screenshots/20.png)
![Resolved](screenshots/21.png)
