# User Not Added to Security Group

## Summary
User unable to perform administrative actions due to missing group membership.

## User
Kevin Patel

## Department
IT (System Administrator)

## Issue
User reports inability to run applications with administrative privileges.  
User expected to have elevated access based on role.

---

## Troubleshooting
- Reviewed user-reported privilege issue
- Identified failure when attempting to run application as administrator
- Determined issue related to insufficient permissions
- Accessed Active Directory Users and Computers
- Navigated to IT Organizational Unit (OU)
- Located user account
- Opened account properties
- Navigated to "Member Of" tab
- Reviewed group memberships
- Identified user only part of "Domain Users" group
- Determined missing "Domain Admins" group membership
- Added missing required security group membership for role-based access
- Applied updated group membership

---

## Resolution
- Added user to required security group
- Applied group membership changes
- Verified elevated privileges assigned
- Confirmed user can run applications as administrator
- Validated successful execution using admin credentials

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

### 4. Issue Resolved (Working State)
![Resolved](screenshots/21.png)
![Resolved](screenshots/22.png)
![Resolved](screenshots/23.png)
![Resolved](screenshots/24.png)
![Resolved](screenshots/25.png)
![Resolved](screenshots/26.png)
![Resolved](screenshots/27.png)
