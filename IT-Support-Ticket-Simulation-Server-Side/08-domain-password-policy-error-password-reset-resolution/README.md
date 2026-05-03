# Domain Password Policy Error – Password Reset and Policy Correction

## Summary
User unable to properly manage password due to incorrect account settings.

## User
Anthony Walker

## Department
Marketing

## Issue
User reports not being prompted to change password at first logon.  
User also experiences frequent login issues due to complex password requirements.

---

## Troubleshooting
- Reviewed user-reported password issue
- Accessed Active Directory Users and Computers
- Navigated to Marketing Organizational Unit (OU)
- Located user account
- Opened account properties
- Navigated to Account settings
- Verified "User must change password at next logon" was disabled
- Verified "User cannot change password" was enabled
- Identified misconfigured password policy settings
- Updated account options to allow password change
- Enabled password change at next logon
- Reset user password

---

## Resolution
- Enabled "User must change password at next logon"
- Disabled "User cannot change password"
- Reset user password to temporary credential
- Allowed user to create new password
- Confirmed successful login with updated credentials

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

