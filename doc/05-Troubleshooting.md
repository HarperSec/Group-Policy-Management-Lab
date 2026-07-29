# Troubleshooting Group Policy Issues

## Overview

During the Group Policy configuration process, several common issues can prevent policies from applying correctly. This section documents troubleshooting methods used to verify Group Policy functionality.

## Issue: Group Policy Was Not Applying

### Problem

The Security Logon Banner policy was initially not appearing on the Windows 11 client after configuration.

### Investigation

The following areas were checked:

* The GPO was correctly created
* The GPO settings were configured
* The GPO was linked to the correct Organizational Unit
* The Windows 11 computer account was located in the correct OU

## Resolution

The issue was resolved by creating a dedicated Workstations Organizational Unit and moving the Windows 11 computer account into that OU.

The Security Logon Banner GPO was then linked to the Workstations OU.

After forcing a Group Policy update:

```cmd
gpupdate /force
```

the policy successfully applied.

## Verification Commands

The following command was used to verify applied policies:

```cmd
gpresult /r
```

This confirmed that the Security Logon Banner GPO was successfully applied to the Windows 11 workstation.

## Lessons Learned

This troubleshooting process demonstrated the importance of:

* Understanding the difference between User Configuration and Computer Configuration policies
* Proper Organizational Unit design
* Verifying GPO scope and linking
* Using built-in Windows troubleshooting commands
