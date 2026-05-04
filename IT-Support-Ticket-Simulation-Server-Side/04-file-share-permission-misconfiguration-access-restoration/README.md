# File Share Permission Misconfiguration – Access Restoration

## Summary
Access denied to network share caused by missing Active Directory security group membership (RBAC misconfiguration), not NTFS or share permission errors.

## User
Emily Rodriguez

## Department
Marketing

## Issue
User unable to access mapped network drive (Z:).  
Error: *“You do not have permission to access \\FILESERVER01\Marketing\.”*

---

## Troubleshooting
- Validated **access denied** error on network share  
- Initially suspected **NTFS/share permission misconfiguration**  
- Reviewed **Share Permissions** and **NTFS permissions** on file server  
- Confirmed correct access assigned to **Marketing Team security group**  
- Identified mismatch between assigned permissions and user access  
- Accessed **Active Directory Users and Computers (ADUC)**  
- Navigated to **Marketing OU** and reviewed **Marketing Team security group**  
- Verified user was **not a member of the required security group**  
- Identified root cause as **RBAC/group membership misconfiguration**  
- Added user to **Marketing Team security group**  

---

## Resolution
- Restored access by assigning user to correct **Active Directory security group**  
- Ensured alignment with **role-based access control (RBAC)** model  
- Validated fix by having user reattempt access to network share  
- Confirmed successful access to shared folder and contents  

---

## Screenshots

### 1. Ticket (Spiceworks)
![Ticket](screenshots/1.png)

### 2. Reported Issue
![Issue](screenshots/2.png)

### 3. Troubleshooting Steps
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
![Troubleshooting](screenshots/24.png)
![Troubleshooting](screenshots/25.png)
![Troubleshooting](screenshots/26.png)
![Troubleshooting](screenshots/27.png)
![Troubleshooting](screenshots/28.png)
![Troubleshooting](screenshots/29.png)

### 4. Issue Resolved (Working State)
![Resolved](screenshots/30.png)
![Resolved](screenshots/31.png)
![Resolved](screenshots/32.png)
![Resolved](screenshots/33.png)
![Resolved](screenshots/34.png)
