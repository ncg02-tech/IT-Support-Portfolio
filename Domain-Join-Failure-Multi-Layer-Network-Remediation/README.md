# Enterprise Domain Join Failure – Multi-Layer Network Remediation

## Overview
Diagnosed and resolved a complex Active Directory domain join failure in a Windows Server and Windows 11 virtual lab environment. The issue required multi-layer troubleshooting across DNS configuration, firewall policy, network reachability, LDAP connectivity, and network profile settings before the client workstation could successfully join the domain.

---

## Environment / Tech Stack
- Oracle VirtualBox
- Windows Server 2025 (Domain Controller)
- Windows 11 (Client Workstation)
- Active Directory Domain Services (AD DS)
- DNS
- LDAP
- Windows Defender Firewall with Advanced Security
- Windows PowerShell
- Command Prompt
- TCP/IP Networking

---

## Issue
Windows 11 client workstation failed to join the `lab4home.local` Active Directory domain.

Error displayed:

> “An Active Directory Domain Controller (AD DC) for the domain `lab4home.local` could not be contacted.”

---

## Troubleshooting

### Initial Domain Join Failure
- Verified client workstation was using a local account context
- Confirmed workstation was not joined to a domain
- Attempted to join domain `lab4home.local`
- Received Active Directory Domain Controller discovery failure

### DNS Configuration Remediation
- Ran `ipconfig /all` to review client network configuration
- Identified incorrect DNS server assignment
- Changed DNS configuration from automatic to manual
- Set client DNS server to the Domain Controller IP address: `10.0.0.55`
- Flushed DNS resolver cache using `ipconfig /flushdns`
- Re-ran `ipconfig /all` to confirm DNS configuration updated correctly

### Continued Domain Join Failure
- Retried domain join after correcting DNS configuration
- Confirmed domain join still failed with the same AD DC discovery error

### Network Connectivity Testing
- Tested connectivity to Domain Controller using `ping 10.0.0.55`
- Received `General Failure`, indicating local communication failure
- Verified default gateway connectivity using `ping 10.0.0.1`
- Confirmed external connectivity using `ping 8.8.8.8`
- Ran `nslookup lab4home.local` and confirmed DNS request timeout
- Ran `tracert 10.0.0.55` and received `General Failure`
- Determined issue was not general internet connectivity or gateway failure

### Firewall Policy Remediation
- Opened Windows Defender Firewall with Advanced Security
- Reviewed outbound firewall rules
- Identified outbound rule blocking traffic to Domain Controller IP `10.0.0.55`
- Removed restrictive outbound firewall rule
- Retested connectivity to Domain Controller
- Confirmed successful ICMP response using `ping`
- Confirmed network path using `tracert`

### LDAP Connectivity and Network Profile Remediation
- Retried domain join after firewall remediation
- Confirmed domain join still failed
- Opened Windows PowerShell for deeper connectivity testing
- Ran `Get-NetConnectionProfile`
- Identified client network profile was set to Public
- Ran `Test-NetConnection 10.0.0.55 -Port 389`
- Confirmed LDAP connectivity failure with `TcpTestSucceeded : False`
- Changed network profile from Public to Private
- Re-ran `Test-NetConnection 10.0.0.55 -Port 389`
- Confirmed LDAP connectivity succeeded with `TcpTestSucceeded : True`

---

## Resolution
- Corrected client DNS server IP configuration to point to the Domain Controller
- Cleared DNS cache and validated updated DNS settings
- Removed outbound firewall rule blocking communication to the Domain Controller
- Verified successful ICMP and route connectivity to the Domain Controller
- Changed network profile from Public to Private
- Validated LDAP connectivity on port `389`
- Successfully joined Windows 11 client to `lab4home.local`
- Restarted workstation and confirmed domain authentication
- Logged in using domain credentials to verify successful domain integration

---

## Key Skills Demonstrated
- Active Directory Domain Join Troubleshooting
- DNS Client Configuration
- Domain Controller Discovery
- LDAP Connectivity Testing
- Windows Firewall Rule Analysis
- Network Profile Remediation
- TCP/IP Troubleshooting
- Command-Line Network Diagnostics
- PowerShell Network Diagnostics
- Root Cause Analysis
- Enterprise Endpoint Integration

---

## Key Takeaways
- Active Directory domain joins depend heavily on proper DNS configuration
- Firewall rules can block domain communication even when internet access works
- Public network profiles can interfere with network discoverability and domain services
- LDAP connectivity testing helps validate communication with the Domain Controller
- Complex domain join failures require layered troubleshooting across DNS, firewall, network, and authentication services

---

## Screenshots

### 1. Initial Local Account State and Domain Join Failure
![Initial Domain Join Failure](screenshots/1.png)
![Initial Domain Join Failure](screenshots/2.png)
![Initial Domain Join Failure](screenshots/3.png)
![Initial Domain Join Failure](screenshots/4.png)
![Initial Domain Join Failure](screenshots/5.png)
![Initial Domain Join Failure](screenshots/6.png)
![Initial Domain Join Failure](screenshots/7.png)
![Initial Domain Join Failure](screenshots/8.png)
![Initial Domain Join Failure](screenshots/9.png)
![Initial Domain Join Failure](screenshots/10.png)
![Initial Domain Join Failure](screenshots/11.png)

### 2. DNS Misconfiguration Identification and Correction
![DNS Misconfiguration](screenshots/12.png)
![DNS Misconfiguration](screenshots/13.png)
![DNS Misconfiguration](screenshots/14.png)
![DNS Misconfiguration](screenshots/15.png)
![DNS Misconfiguration](screenshots/16.png)
![DNS Misconfiguration](screenshots/17.png)
![DNS Misconfiguration](screenshots/18.png)
![DNS Misconfiguration](screenshots/19.png)
![DNS Misconfiguration](screenshots/20.png)
![DNS Misconfiguration](screenshots/21.png)
![DNS Misconfiguration](screenshots/22.png)
![DNS Misconfiguration](screenshots/23.png)
![DNS Misconfiguration](screenshots/24.png)
![DNS Misconfiguration](screenshots/25.png)
![DNS Misconfiguration](screenshots/26.png)
![DNS Misconfiguration](screenshots/27.png)

### 3. DNS Cache Flush and Configuration Validation
![DNS Validation](screenshots/28.png)
![DNS Validation](screenshots/29.png)
![DNS Validation](screenshots/30.png)
![DNS Validation](screenshots/31.png)
![DNS Validation](screenshots/32.png)
![DNS Validation](screenshots/33.png)
![DNS Validation](screenshots/34.png)

### 4. Continued Domain Join Failure After DNS Correction
![Continued Domain Join Failure](screenshots/35.png)
![Continued Domain Join Failure](screenshots/36.png)
![Continued Domain Join Failure](screenshots/37.png)
![Continued Domain Join Failure](screenshots/38.png)
![Continued Domain Join Failure](screenshots/39.png)
![Continued Domain Join Failure](screenshots/40.png)
![Continued Domain Join Failure](screenshots/41.png)
![Continued Domain Join Failure](screenshots/42.png)
![Continued Domain Join Failure](screenshots/43.png)
![Continued Domain Join Failure](screenshots/44.png)

### 5. Network Connectivity Testing and Root Cause Isolation
![Network Connectivity Testing](screenshots/45.png)
![Network Connectivity Testing](screenshots/46.png)
![Network Connectivity Testing](screenshots/47.png)
![Network Connectivity Testing](screenshots/48.png)
![Network Connectivity Testing](screenshots/49.png)
![Network Connectivity Testing](screenshots/50.png)
![Network Connectivity Testing](screenshots/51.png)
![Network Connectivity Testing](screenshots/52.png)
![Network Connectivity Testing](screenshots/53.png)
![Network Connectivity Testing](screenshots/54.png)
![Network Connectivity Testing](screenshots/55.png)
![Network Connectivity Testing](screenshots/56.png)
![Network Connectivity Testing](screenshots/57.png)
![Network Connectivity Testing](screenshots/58.png)

### 6. Outbound Firewall Rule Identification and Removal
![Firewall Rule Remediation](screenshots/59.png)
![Firewall Rule Remediation](screenshots/60.png)
![Firewall Rule Remediation](screenshots/61.png)
![Firewall Rule Remediation](screenshots/62.png)
![Firewall Rule Remediation](screenshots/63.png)
![Firewall Rule Remediation](screenshots/64.png)
![Firewall Rule Remediation](screenshots/65.png)
![Firewall Rule Remediation](screenshots/66.png)
![Firewall Rule Remediation](screenshots/67.png)

### 7. Connectivity Validation After Firewall Remediation
![Connectivity Restored](screenshots/68.png)
![Connectivity Restored](screenshots/69.png)
![Connectivity Restored](screenshots/70.png)
![Connectivity Restored](screenshots/71.png)
![Connectivity Restored](screenshots/72.png)

### 8. Continued Domain Join Failure and LDAP Network Profile Testing
![LDAP and Network Profile Testing](screenshots/73.png)
![LDAP and Network Profile Testing](screenshots/74.png)
![LDAP and Network Profile Testing](screenshots/75.png)
![LDAP and Network Profile Testing](screenshots/76.png)
![LDAP and Network Profile Testing](screenshots/77.png)
![LDAP and Network Profile Testing](screenshots/78.png)
![LDAP and Network Profile Testing](screenshots/79.png)
![LDAP and Network Profile Testing](screenshots/80.png)
![LDAP and Network Profile Testing](screenshots/81.png)
![LDAP and Network Profile Testing](screenshots/82.png)
![LDAP and Network Profile Testing](screenshots/83.png)
![LDAP and Network Profile Testing](screenshots/84.png)
![LDAP and Network Profile Testing](screenshots/85.png)
![LDAP and Network Profile Testing](screenshots/86.png)
![LDAP and Network Profile Testing](screenshots/87.png)
![LDAP and Network Profile Testing](screenshots/88.png)

### 9. LDAP Connectivity Restored and Successful Domain Join
![Successful Domain Join](screenshots/89.png)
![Successful Domain Join](screenshots/90.png)
![Successful Domain Join](screenshots/91.png)
![Successful Domain Join](screenshots/92.png)
![Successful Domain Join](screenshots/93.png)
![Successful Domain Join](screenshots/94.png)
![Successful Domain Join](screenshots/95.png)
![Successful Domain Join](screenshots/96.png)

### 10. Domain Join Verification and Domain Login
![Domain Join Verification](screenshots/97.png)
![Domain Join Verification](screenshots/98.png)
![Domain Join Verification](screenshots/99.png)
![Domain Join Verification](screenshots/100.png)
