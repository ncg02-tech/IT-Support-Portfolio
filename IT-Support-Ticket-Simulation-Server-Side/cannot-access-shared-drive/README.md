# Cannot Access Shared Drive

## Summary
User unable to access shared network drive due to permission issue.

## User
Emily Rodriguez

## Department
Marketing

## Issue
User reports inability to access shared drive (Z:).  
Error displayed: "You do not have permission to access \\FILESERVER01\Marketing\."

---

## Troubleshooting
- Reviewed user-reported permission error
- Identified access denied message on shared drive
- Accessed file server hosting shared directory
- Opened folder properties
- Navigated to Sharing tab and Advanced Sharing settings
- Reviewed share permissions
- Identified missing "Domain Users" group in share permissions
- Added "Domain Users" with read access
- Navigated to Security tab
- Reviewed NTFS permissions
- Identified missing "Domain Users" group
- Added "Domain Users" with read and execute permissions
- Applied all permission changes

---

## Resolution
- Added "Domain Users" to share permissions
- Added "Domain Users" to NTFS security permissions
- Applied correct access levels (Read, List Folder Contents, Read & Execute)
- Confirmed user can access shared drive
- Verified folder contents visible on client machine

---

## Screenshots

### 1. Ticket (Spiceworks)
![Ticket](screenshots/ticket.png)

### 2. Reported Issue
![Issue](screenshots/issue.png)

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
