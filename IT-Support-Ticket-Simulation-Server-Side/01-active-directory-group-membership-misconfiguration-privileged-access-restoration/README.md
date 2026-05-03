# Active Directory Group Membership Misconfiguration – Privileged Access Restoration

## Summary
Administrative access failure caused by incorrect Active Directory group membership (RBAC misconfiguration).

## User
Kevin Patel

## Department
IT (System Administrator)

## Issue
User unable to authenticate to Domain Controller and perform administrative tasks due to missing privileged group membership.

---

## Troubleshooting
- Reviewed access failure and identified insufficient privileges  
- Logged in with elevated administrative account  
- Accessed **Active Directory Users and Computers (ADUC)**  
- Located user within IT OU and reviewed **group membership**  
- Confirmed user only assigned to **Domain Users**  
- Identified missing delegated administrative role  
- Selected **Account Operators** based on least-privilege model  
- Added user to appropriate security group  
- Re-authenticated with user account  
- Verified Domain Controller access and AD management capability  
- Validated effective permissions using `whoami /groups`  

---

## Resolution
- Assigned user to **Account Operators** security group  
- Restored administrative access using **least privilege principles**  
- Confirmed Domain Controller login and directory management functionality  
- Verified group membership and permissions via command-line validation  

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
