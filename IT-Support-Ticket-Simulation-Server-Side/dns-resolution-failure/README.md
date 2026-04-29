# DNS Resolution Failure

## Summary
User unable to access internal website via hostname due to DNS resolution issue.

## User
Michael Thompson

## Department
Operations

## Issue
User reports inability to access internal site using hostname.  
User confirms site is accessible when using IP address.

---

## Troubleshooting
- Reviewed user-reported access behavior
- Identified hostname resolution failure with IP access working
- Determined issue related to DNS resolution
- Opened Command Prompt on client machine
- Tested connectivity using hostname (ping failed)
- Tested connectivity using IP address (ping successful)
- Accessed Domain Controller
- Opened DNS Manager
- Navigated to Forward Lookup Zones
- Reviewed existing DNS records
- Identified missing A record for web server
- Created new A record for "web" (web.homelab.local)
- Verified DNS record creation

---

## Resolution
- Created missing A record in DNS Manager
- Mapped hostname to correct IP address
- Verified hostname resolution using Command Prompt
- Confirmed internal website accessible via hostname
- User access restored

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
![Troubleshooting](screenshots/troubleshooting15.png)

### 4. Issue Resolved (Working State)
![Resolved](screenshots/resolved1.png)
![Resolved](screenshots/resolved2.png)
