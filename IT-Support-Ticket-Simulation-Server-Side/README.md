# IT Support Ticket Simulation (Server-Side)

## Project Overview
Simulated enterprise-level IT support scenarios within a Windows Server Active Directory environment. This project focuses on identity and access management (IAM), domain services, authentication troubleshooting, and file server permission control.

Demonstrates hands-on experience managing user accounts, enforcing access policies, troubleshooting domain-related issues, and maintaining secure and functional enterprise environments.

---

## Environment / Tools
- Windows Server (Domain Controller)
- Active Directory Domain Services (AD DS)
- DNS Manager
- File Server (NTFS & Share Permissions)
- Group Membership / Role-Based Access Control (RBAC)
- Command Prompt (`whoami /groups`)
- Spiceworks Help Desk
- Windows Administrative Tools

---

## Skills Demonstrated
- Active Directory User & Group Management  
- Identity & Access Management (IAM)  
- Role-Based Access Control (RBAC)  
- Authentication & Authorization Troubleshooting  
- DNS Record Management (A Records)  
- NTFS & Share Permission Configuration  
- Access Control Remediation (Under/Over-Permissioning)  
- Account Lifecycle Management (Provisioning → Access → Restrictions)  
- Policy-Based Access Control (Logon Hours, Password Policies)  
- Root Cause Analysis & Validation  

---

## Featured Enterprise Scenarios

- [Active Directory Group Membership Misconfiguration – Privileged Access Restoration](./01-active-directory-group-membership-misconfiguration-privileged-access-restoration)  
- [Domain Account Lockout – Password Reset and Access Restoration](./02-domain-account-lockout-password-reset-and-access-restoration)  
- [DNS Record Misconfiguration – Missing A Record Resolution](./03-dns-record-misconfiguration-missing-a-record-resolution)  
- [File Share Permission Misconfiguration – Access Restoration](./04-file-share-permission-misconfiguration-access-restoration)  

---

## Ticket Breakdown

### Identity & Access Management (Active Directory)

- [Active Directory Group Membership Misconfiguration – Privileged Access Restoration](./01-active-directory-group-membership-misconfiguration-privileged-access-restoration)  
- [Domain Account Lockout – Password Reset and Access Restoration](./02-domain-account-lockout-password-reset-and-access-restoration)  
- [Active Directory Disabled Account – Access Restoration](./07-active-directory-disabled-account-access-restoration)  
- [Domain Authentication Failure – Password Reset Resolution](./09-domain-authentication-failure-password-reset-resolution)  

---

### Access Control & Security (Permissions)

- [File Share Permission Misconfiguration – Access Restoration](./04-file-share-permission-misconfiguration-access-restoration)  
- [Overprovisioned File Share Permissions – Unauthorized Access Remediation](./05-overprovisioned-file-share-permission-unauthorized-access-remediation)  

---

### DNS & Infrastructure

- [DNS Record Misconfiguration – Missing A Record Resolution](./03-dns-record-misconfiguration-missing-a-record-resolution)  

---

### Policy & Account Configuration

- [Domain Logon Hours Restriction – Policy Adjustment](./06-domain-logon-hours-policy-restriction-adjustment)  
- [Domain Password Policy Error – Password Reset and Policy Correction](./08-domain-password-policy-error-password-reset-resolution)  

---

### Account Lifecycle Management

- [Active Directory User Onboarding – Account Provisioning](./10-active-directory-user-onboarding-account-provisioning)  

---

## Troubleshooting Methodology

Each scenario follows a structured enterprise troubleshooting approach:

1. Identify and validate the reported issue  
2. Reproduce the issue within the domain environment  
3. Analyze authentication, authorization, or configuration behavior  
4. Isolate root cause (permissions, policy, DNS, or account state)  
5. Apply targeted remediation aligned with least privilege principles  
6. Validate resolution through system testing and user confirmation  
7. Document steps, findings, and outcomes  

---

## Key Takeaways
- Identity and access issues often stem from misconfigured group memberships and policies  
- Proper permission design requires balancing functionality with least privilege principles  
- DNS misconfigurations can directly impact internal service availability  
- Authentication failures must be differentiated between credential, policy, and account state issues  
- Structured troubleshooting significantly reduces resolution time in enterprise environments  

---

## Notes
All scenarios were intentionally created and resolved in a controlled lab environment to simulate real-world enterprise IT support operations.
