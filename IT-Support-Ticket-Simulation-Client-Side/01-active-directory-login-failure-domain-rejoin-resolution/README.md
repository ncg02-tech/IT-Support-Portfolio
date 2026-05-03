# Active Directory Login Failure – Domain Rejoin

## Summary
Authentication failure caused by workstation not joined to Active Directory domain.

## User
Olivia Martinez

## Department
HR

## Issue
User unable to authenticate with domain credentials.  
System presenting local login context instead of domain authentication.

---

## Troubleshooting
- Validated login failure using domain credentials  
- Identified system authenticating against **local account context**  
- Determined workstation not joined to domain  
- Authenticated using **local administrator account**  
- Accessed system configuration and domain membership settings  
- Initiated domain join using administrative credentials  
- Restarted system to apply domain configuration  

---

## Resolution
- Rejoined workstation to Active Directory domain  
- Restored domain authentication functionality  
- Verified domain login prompt and successful user authentication  

---

## Screenshots

### 1. Ticket (Spiceworks)
![Ticket](screenshots/ticket.png)

### 2. Reported Issue
![Issue](screenshots/1.png)
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

### 4. Issue Resolved (Working State)
![Resolved](screenshots/17.png)
![Resolved](screenshots/18.png)
![Resolved](screenshots/19.png)
