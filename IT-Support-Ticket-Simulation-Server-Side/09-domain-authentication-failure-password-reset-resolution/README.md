# Domain Authentication Failure – Password Reset Resolution

## Summary
Authentication failure caused by invalid user credentials in Active Directory.

## User
Alicia Brown

## Department
HR

## Issue
User unable to authenticate with error: *“The user name or password is incorrect.”*  
User reports credentials believed to be correct.

---

## Troubleshooting
- Reviewed authentication failure and validated error message  
- Accessed **Active Directory Users and Computers (ADUC)**  
- Located user account and reviewed account status  
- Confirmed no lockout, restriction, or disabled conditions  
- Isolated issue to **credential mismatch (password issue)**  
- Determined password reset required  

---

## Resolution
- Reset user password in Active Directory  
- Restored valid credentials  
- Verified successful authentication on domain-joined system  

---

## Screenshots

### 1. Ticket (Spiceworks)
![Ticket](screenshots/ticket.png)

### 2. Reported Issue
![Issue](screenshots/issue1.png)
![Issue](screenshots/issue2.png)

### 3. Troubleshooting Steps
![Troubleshooting](screenshots/troubleshooting1.png)
![Troubleshooting](screenshots/troubleshooting2.png)
![Troubleshooting](screenshots/troubleshooting3.png)
![Troubleshooting](screenshots/troubleshooting4.png)
![Troubleshooting](screenshots/troubleshooting5.png)
![Troubleshooting](screenshots/troubleshooting6.png)
![Troubleshooting](screenshots/troubleshooting7.png)
![Troubleshooting](screenshots/troubleshooting8.png)
![Troubleshooting](screenshots/troubleshooting9.png)
![Troubleshooting](screenshots/troubleshooting10.png)
![Troubleshooting](screenshots/troubleshooting11.png)
![Troubleshooting](screenshots/troubleshooting12.png)
![Troubleshooting](screenshots/troubleshooting13.png)
![Troubleshooting](screenshots/troubleshooting14.png)

### 4. Issue Resolved (Working State)
![Resolved](screenshots/resolved1.png)
![Resolved](screenshots/resolved2.png)
![Resolved](screenshots/resolved3.png)
