# Overprovisioned File Share Permissions – Unauthorized Access Remediation

## Summary
Unauthorized access caused by overprovisioned file share permissions in Active Directory environment.

## User
Brian Lee

## Department
Operations

## Issue
User has unintended access to restricted Finance directory, violating role-based access control (RBAC) and least privilege principles.

---

## Troubleshooting
- Validated unauthorized access to restricted folder  
- Confirmed access not aligned with user role/department  
- Accessed file server and reviewed **share permissions**  
- Identified user explicitly granted access  
- Determined root cause as **overprovisioned permissions**  

---

## Resolution
- Removed unauthorized access from share permissions  
- Enforced **least privilege access model**  
- Verified restricted folder no longer visible or accessible  
- Confirmed access control aligned with department roles  

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

### 4. Issue Resolved (Working State)
![Resolved](screenshots/18.png)
![Resolved](screenshots/19.png)
![Resolved](screenshots/20.png)
![Resolved](screenshots/21.png)
![Resolved](screenshots/22.png)
![Resolved](screenshots/23.png)
![Resolved](screenshots/24.png)
![Resolved](screenshots/25.png)
![Resolved](screenshots/26.png)
