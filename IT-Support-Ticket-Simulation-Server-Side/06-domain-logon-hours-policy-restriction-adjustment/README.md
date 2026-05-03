# Domain Logon Hours Restriction – Policy Adjustment

## Summary
Authentication failure caused by Active Directory logon hours policy restricting user access outside approved timeframe.

## User
Marcus Johnson

## Department
Operations

## Issue
User unable to authenticate after business hours despite valid credentials.  
Access restricted by configured logon hours policy.

---

## Troubleshooting
- Validated login failure during restricted time window  
- Identified issue as **policy-based access restriction (logon hours)**  
- Accessed **Active Directory Users and Computers (ADUC)**  
- Located user account and reviewed **Logon Hours configuration**  
- Confirmed access limited to standard business hours  
- Determined requirement for extended access window  

---

## Resolution
- Updated **logon hours policy** to include approved timeframe  
- Applied changes to user account in Active Directory  
- Restored authentication access outside standard hours  
- Verified successful login and policy enforcement  

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
![Troubleshooting](screenshots/17.png)
![Troubleshooting](screenshots/18.png)
![Troubleshooting](screenshots/19.png)
![Troubleshooting](screenshots/20.png)

### 4. Issue Resolved (Working State)
![Resolved](screenshots/21.png)
![Resolved](screenshots/22.png)
![Resolved](screenshots/23.png)
