# IT-HelpDesk-HomeLab
Hands-on IT Help Desk troubleshooting projects using Windows Server, Active Directory, Windows 11, and VirtualBox.


## Home Lab Environment

I built and configured a virtual IT environment using Oracle VirtualBox to practice real-world Help Desk and system administration tasks.

- **DC01:** Windows Server configured with Active Directory Domain Services and DNS.
- **PC01:** Windows 11 Pro workstation joined to the aguilartech.local domain.
- **Networking:** Configured virtual network adapters, static IP addressing, and DNS settings to enable communication between both machines.
- **Active Directory:** Created organizational units, employee accounts, and security groups.
- **File Sharing:** Configured shared folders and NTFS permissions to manage user access.
- **Troubleshooting:** Used the environment to simulate and resolve common IT support issues involving user accounts, network connectivity, permissions, and system performance.

All projects below were completed in this self-built virtual environment.


## Completed Help Desk Projects

### [Ticket HD-001: Active Directory Account Lockout](01-Account-Lockout/README.md)

**Status:** Resolved

Simulated an employee account lockout, investigated the issue using Active Directory, restored account access, and verified successful login on a domain-joined Windows 11 workstation.

**Skills:** Active Directory, Group Policy, Windows authentication, account troubleshooting.

### [Ticket HD-002: New Employee Account Setup](02-New-Employee-Setup/README.md)

**Status:** Completed (password-change issue documented)

Created a new employee account in Active Directory, assigned the appropriate Sales security group, troubleshot DNS name resolution, and verified access to a shared network folder.

**Skills:** Active Directory, user provisioning, security groups, DNS troubleshooting, shared-folder permissions, Windows 11.

### [Ticket HD-003: Shared Folder Permission Troubleshooting](03-Shared-Folder-Permissions/README.md)

**Status:** Resolved

Investigated an employee's inability to modify files in a shared network folder. Identified restricted NTFS permissions, restored Modify access through the Sales security group, and verified successful file creation and modification.

**Skills:** NTFS permissions, Active Directory security groups, network shares, least privilege, access troubleshooting.


### [Ticket HD-004: DNS Resolution Troubleshooting](04-DNS-Troubleshooting/README.md)

**Status:** Resolved

Simulated a DNS misconfiguration that prevented a Windows 11 workstation from resolving the domain controller's hostname. Used ping, nslookup, and ipconfig to diagnose the issue, corrected the DNS server address, and verified successful hostname resolution.

**Skills:** DNS troubleshooting, TCP/IP networking, Windows network configuration, Command Prompt, connectivity testing.


### [Ticket HD-005: Windows Performance Troubleshooting](05-Windows-Performance-Troubleshooting/README.md)

**Status:** Resolved

Simulated a slow Windows 11 computer by increasing browser resource usage. Used Task Manager to investigate CPU, memory, and disk activity, identified Microsoft Edge consuming 97.5% CPU, and restored performance by closing unnecessary browser workloads.

**Skills:** Windows 11 troubleshooting, Task Manager, CPU and RAM monitoring, process analysis, performance optimization, end-user support.
