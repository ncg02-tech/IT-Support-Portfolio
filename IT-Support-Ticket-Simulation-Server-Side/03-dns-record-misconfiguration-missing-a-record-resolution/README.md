# DNS Record Misconfiguration – Missing A Record Resolution

## Summary
Hostname resolution failure caused by missing DNS A record within the internal domain.

## User
Michael Thompson

## Department
Operations

## Issue
User unable to access internal web service via hostname.  
Service accessible via IP address, indicating DNS resolution failure.

---

## Troubleshooting
- Validated issue: hostname unreachable, IP reachable  
- Executed connectivity tests (`ping`) to confirm DNS failure  
- Identified issue isolated to **name resolution (not network connectivity)**  
- Accessed Domain Controller and opened **DNS Manager**  
- Reviewed **Forward Lookup Zone** records  
- Identified missing A record for internal web host  
- Created A record mapping hostname to correct IP  

---

## Resolution
- Added missing **DNS A record** for internal web server  
- Restored hostname-to-IP resolution  
- Verified successful name resolution via command line  
- Confirmed internal site accessibility using hostname  

---

## Screenshots

### 1. Ticket (Spiceworks)
![Ticket](screenshots/ticket.png)

### 2. Reported Issue
![Issue](screenshots/issue1.png)
![Issue](screenshots/issue2.png)

### 3. Troubleshooting Steps
![Troubleshooting](screenshots/troubleshooting1.png)
![Troubleshooting](screenshots/troubleshooting1a.png)
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
