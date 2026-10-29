# IT-HelpDesk-HomeLab
Hands-on IT Help Desk troubleshooting projects using Windows Server, Active Directory, Windows 11, and VirtualBox.

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
