# File Share Permission Misconfiguration – Access Restoration

## Summary
Access denied to network share caused by misconfigured NTFS and share permissions.

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
- Accessed file server and reviewed folder **Share Permissions**  
- Identified missing **Domain Users** group in share configuration  
- Added appropriate read-level share permissions  
- Reviewed **NTFS (Security) permissions**  
- Identified missing access control entry for Domain Users  
- Applied **Read & Execute** permissions at NTFS level  
- Ensured alignment between share and NTFS permissions  

---

## Resolution
- Remediated permission misconfiguration at both **share and NTFS layers**  
- Restored user access following proper permission hierarchy  
- Verified successful access to network drive and folder contents  

---

## Screenshots

### 1. Ticket (Spiceworks)
![Ticket](screenshots/ticket.png)

### 2. Reported Issue
![Issue](screenshots/issue.png)

### 3. Troubleshooting Steps
![Troubleshooting](screenshots/troubleshooting0.png)
![Troubleshooting](screenshots/troubleshooting0a.png)
![Troubleshooting](screenshots/troubleshooting0b.png)
![Troubleshooting](screenshots/troubleshooting0c.png)
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
![Troubleshooting](screenshots/troubleshooting15.png)

### 4. Issue Resolved (Working State)
![Resolved](screenshots/resolved0.png)
![Resolved](screenshots/resolved0a.png)
![Resolved](screenshots/resolved0b.png)
![Resolved](screenshots/resolved1.png)
![Resolved](screenshots/resolved2.png)
