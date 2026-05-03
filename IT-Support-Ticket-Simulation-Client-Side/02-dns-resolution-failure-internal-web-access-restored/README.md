# DNS Resolution Failure – Internal Web Access Restored

## Summary
Internal service access failure caused by incorrect DNS client configuration.

## User
Daniel Foster

## Department
Marketing

## Issue
User unable to access internal web application while external sites remain reachable, indicating DNS resolution issue.

---

## Troubleshooting
- Reproduced issue: internal site unreachable, external connectivity functional  
- Validated network connectivity independent of DNS  
- Executed `ipconfig /all` to review DNS configuration  
- Identified incorrect DNS server assignment (non-domain DNS)  
- Accessed network adapter settings and updated DNS to **internal domain controller**  
- Flushed DNS cache (`ipconfig /flushdns`)  
- Verified hostname resolution and connectivity via command line  

---

## Resolution
- Corrected DNS client configuration to use internal DNS server  
- Restored internal name resolution  
- Verified access to internal web service via hostname  

---

## Screenshots

### 1. Ticket (Spiceworks)
![Ticket](screenshots/ticket.png)

### 2. Reported Issue (Internal Site Not Reachable)
![Issue](screenshots/1.png)

### 3. External Connectivity Verified
![External Connectivity](screenshots/2.png)

### 4. Troubleshooting Steps
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

### 5. Issue Resolved (Working State)
![Resolved](screenshots/30.png)
