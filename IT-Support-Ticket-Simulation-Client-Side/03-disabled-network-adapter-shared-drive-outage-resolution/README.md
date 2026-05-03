# Network Adapter Failure (Shared Drive Outage)

## Summary
Network connectivity failure caused by disabled Ethernet adapter, resulting in loss of access to shared resources.

## User
David Lee

## Department
Operations

## Issue
User unable to access shared network drive due to loss of network connectivity.

---

## Troubleshooting
- Validated shared drive unavailable (mapped drive error)  
- Tested connectivity to file server (`ping`) and identified packet loss  
- Confirmed system offline via network status indicator  
- Isolated issue to **local network configuration**  
- Accessed advanced network settings  
- Identified **disabled Ethernet adapter**  
- Re-enabled adapter and restored network interface  
- Retested connectivity and verified successful response  

---

## Resolution
- Restored network connectivity by enabling Ethernet adapter  
- Re-established communication with file server  
- Verified shared drive accessibility and file visibility  

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
![Troubleshooting](screenshots/17.png)
![Troubleshooting](screenshots/18.png)

### 4. Issue Resolved (Working State)
![Resolved](screenshots/19.png)
![Resolved](screenshots/20.png)
