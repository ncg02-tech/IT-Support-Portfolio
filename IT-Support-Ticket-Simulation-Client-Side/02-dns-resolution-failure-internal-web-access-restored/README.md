# DNS Resolution Failure – Internal Web Access Restored

## Summary
User unable to access internal company website.

## User
Daniel Foster

## Department
Marketing

## Issue
User reports that the internal company website does not load, while external websites function normally.

---

## Troubleshooting
- Reproduced issue by accessing internal website
- Verified external connectivity (Google reachable)
- Checked network configuration using ipconfig /all
- Identified incorrect DNS server assignment
- Accessed Network Adapter settings
- Modified DNS configuration to internal DNS server
- Flushed DNS resolver cache
- Tested name resolution and connectivity using ping

---

## Resolution
- Updated client DNS server to internal domain controller
- Cleared DNS cache using ipconfig /flushdns
- Verified connectivity to internal web server (web.homelab.local)
- Confirmed internal website loads successfully in browser

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
