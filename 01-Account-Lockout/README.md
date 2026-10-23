# Help Desk Ticket 01 - Active Directory Account Lockout

**Ticket ID:** HD-001  
**Status:** Resolved  
**Category:** User Account / Authentication  
**Environment:** Windows Server, Windows 11 Pro, Active Directory, Oracle VirtualBox

## Issue Description

A simulated employee, Daniel Martinez from the Sales department, was unable to sign into his Windows 11 computer due to an account lockout.

The goal of this lab was to practice troubleshooting account lockouts in Active Directory, identifying the issue, restoring access, and verifying the solution.

## Lab Environment

- **DC01:** Windows Server running Active Directory Domain Services
- **PC01:** Windows 11 Pro domain-joined workstation
- **Domain:** aguilartech.local
- **User Account:** dmartinez
- **Virtualization:** Oracle VirtualBox

## Troubleshooting Steps

### 1. Checked the Account Lockout Policy

Opened Group Policy Management on DC01 and reviewed the Default Domain Policy.

The account lockout settings were:

- Account lockout threshold: 5 failed login attempts
- Account lockout duration: 10 minutes
- Reset account lockout counter after: 10 minutes

This helped me understand when an account would become locked and how long the lockout would last.

### 2. Reproduced the Issue

On PC01, I intentionally entered an incorrect password multiple times while attempting to sign into Daniel Martinez's account.

Windows displayed the message:

"Invalid credentials, delaying next attempt..."

This showed that Windows was delaying additional login attempts after incorrect credentials were entered.

### 3. Investigated the Account in Active Directory

On DC01, I opened Active Directory Users and Computers and located Daniel Martinez's account in the Sales organizational unit.

I opened the account properties and selected the Account tab.

Active Directory displayed a message confirming that the account was currently locked out on the domain controller.

This confirmed that an account lockout was preventing the user from signing in.

### 4. Resolved the Issue

After confirming the lockout, I selected the Unlock account checkbox in the user's account properties and applied the change.

This cleared the account lockout.

### 5. Verified the Solution

Returned to PC01 and attempted to sign in using Daniel Martinez's correct credentials.

The login was successful, confirming that access had been restored.

## Root Cause

The account lockout was intentionally triggered by repeated incorrect password attempts during the lab.

In a real Help Desk environment, I would also investigate whether the failed attempts were caused by forgotten passwords, outdated saved credentials, or another authentication issue.

## What I Learned

This lab helped me practice diagnosing and resolving account lockouts using Active Directory.

I learned how to review account lockout policies, confirm whether a user account is locked, unlock the account, and verify that the user can successfully sign in afterward.

I also learned the importance of confirming the problem before making changes and testing the solution before closing a Help Desk ticket.

## Skills Practiced

- Active Directory Users and Computers
- User account troubleshooting
- Group Policy Management
- Windows authentication
- Account lockout resolution
- Troubleshooting documentation

**Outcome:** Successfully restored access to the simulated employee's account.
