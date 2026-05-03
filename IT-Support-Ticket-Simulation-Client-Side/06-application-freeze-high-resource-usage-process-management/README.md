# Application Freeze – High Resource Usage / Process Management

## Summary
Application unresponsiveness caused by excessive process instances and high resource utilization.

## User
Daniel White

## Department
Operations

## Issue
System becomes unresponsive when launching Notepad due to multiple concurrent instances consuming system resources.

---

## Troubleshooting
- Reproduced issue and observed system freeze behavior  
- Accessed **Task Manager** via secure attention sequence  
- Analyzed **CPU and memory utilization**  
- Identified multiple Notepad processes causing resource contention  
- Isolated root cause to redundant process instances  

---

## Resolution
- Terminated excessive Notepad processes  
- Restarted workstation to stabilize system state  
- Restored normal resource utilization  
- Verified application functionality and system responsiveness  

---

## Screenshots

### 1. Ticket (Spiceworks)
![Ticket](screenshots/ticket.png)

### 2. Reported Issue
![Issue](screenshots/issue1.png)

### 3. Troubleshooting Steps
![Troubleshooting](screenshots/troubleshooting1.png)
![Troubleshooting](screenshots/troubleshooting2.png)
![Troubleshooting](screenshots/troubleshooting3.png)
![Troubleshooting](screenshots/troubleshooting4.png)
![Troubleshooting](screenshots/troubleshooting5.png)

### 4. Issue Resolved (Working State)
![Resolved](screenshots/resolved2.png)
![Resolved](screenshots/resolved3.png)
![Resolved](screenshots/resolved4.png)
