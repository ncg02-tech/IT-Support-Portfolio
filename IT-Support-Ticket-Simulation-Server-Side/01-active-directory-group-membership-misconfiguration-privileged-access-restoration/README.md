# Active Directory Group Membership Misconfiguration – Privileged Access Restoration

## Summary
Administrator unable to perform domain management tasks due to missing security group membership.

## User
Kevin Patel

## Department
IT (System Administrator)

## Issue
Administrator unable to log in to Domain Controller and manage accounts, groups, and computers.  
User lacks required permissions due to missing security group membership.

---

## Troubleshooting
- Reviewed user-reported access issue
- Identified lack of administrative permissions
- Logged in using higher-privileged account
- Accessed Active Directory Users and Computers
- Navigated to IT Organizational Unit (OU)
- Located user account
- Opened account properties
- Reviewed "Member Of" tab
- Identified user only part of "Domain Users" group
- Determined missing administrative group membership
- Evaluated appropriate least-privilege group assignment
- Selected "Account Operators" security group
- Added user to "Account Operators" group
- Applied group membership changes
- Signed out of privileged account
- Attempted login using user credentials
- Verified successful authentication to Domain Controller
- Accessed Active Directory management tools
- Tested ability to manage user accounts
- Disabled test user account to confirm permissions
- Opened Command Prompt
- Executed "whoami /groups"
- Verified membership in "Account Operators" group

---

## Resolution
- Added user to "Account Operators" security group
- Applied least-privilege access model
- Enabled administrative capabilities without over-permissioning
- Verified Domain Controller login access
- Confirmed ability to manage users, groups, and computers
- Validated group membership via command line

---

## Screenshots

### 1. Ticket (Spiceworks)
![Ticket](screenshots/1.png)

### 2. Reported Issue
![Issue](screenshots/2.png)
![Issue](screenshots/3.png)

### 3. Troubleshooting Steps
![Troubleshooting](screenshots/4.png)
![Troubleshooting](screenshots/5.png)
![Troubleshooting](screenshots/6.png)
![Troubleshooting](screenshots/7.png)
![Troubleshooting](screenshots/8.png)
![Troubleshooting](screenshots/9.png)
![Troubleshooting](screenshots/10.png)
![Troubleshooting](screenshots/11.png)
![Troubleshooting](screenshots/12.png)
![Troubleshooting](screenshots/13.png)
![Troubleshooting](screenshots/14.png)
![Troubleshooting](screenshots/15.png)
![Troubleshooting](screenshots/16.png)
![Troubleshooting](screenshots/17.png)
![Troubleshooting](screenshots/18.png)
![Troubleshooting](screenshots/19.png)
![Troubleshooting](screenshots/20.png)
![Troubleshooting](screenshots/21.png)
![Troubleshooting](screenshots/22.png)
![Troubleshooting](screenshots/23.png)

### 4. Issue Resolved (Working State)
![Resolved](screenshots/24.png)
![Resolved](screenshots/25.png)
![Resolved](screenshots/26.png)
![Resolved](screenshots/27.png)
![Resolved](screenshots/28.png)
![Resolved](screenshots/29.png)
![Resolved](screenshots/30.png)
![Resolved](screenshots/31.png)
![Resolved](screenshots/32.png)
![Resolved](screenshots/33.png)
![Resolved](screenshots/34.png)
![Resolved](screenshots/35.png)
![Resolved](screenshots/36.png)
![Resolved](screenshots/37.png)
![Resolved](screenshots/38.png)
![Resolved](screenshots/39.png)
![Resolved](screenshots/40.png)
![Resolved](screenshots/41.png)
