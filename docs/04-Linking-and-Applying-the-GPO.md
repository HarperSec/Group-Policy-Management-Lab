# Linking and Applying the Group Policy Object

## Overview

After creating and configuring the Security Logon Banner Group Policy Object, the GPO was linked to an existing Organizational Unit within the `harper.local` Active Directory domain.

Linking the GPO to an Organizational Unit allows the policy settings to be applied to users and computers located within that OU.

## Linking the GPO

The Security Logon Banner GPO was linked using the Group Policy Management Console.

The GPO was linked to an existing Organizational Unit that contained the test domain user or computer account.

## Group Policy Application Process

After the GPO was linked, Group Policy was updated on the Windows 11 domain-joined client using:

```cmd
gpupdate /force
```

This command forces the client computer to immediately check for and apply updated Group Policy settings.

## Verification

The policy was verified by restarting the Windows 11 client and confirming that the interactive logon message appeared before sign-in.

The successful appearance of the security banner confirmed that:

* The GPO was created correctly
* The GPO was linked to the correct OU
* The Windows 11 client was receiving domain policies
* Active Directory Group Policy processing was functioning correctly

## Screenshots

### GPO Linked to Organizational Unit

[![GPO Linked to OU](path/to/image.png)](https://github.com/HarperSec/Group-Policy-Management-Lab/blob/main/screenshots/04-GPO-Linked-to-OU.png)

### Group Policy Test Result

[![GPO Successfully Applied](path/to/image.png)](https://github.com/HarperSec/Group-Policy-Management-Lab/blob/main/screenshots/05-Logon-Banner-Test-Result.png)  

## Result

The Security Logon Banner Group Policy Object was successfully created, linked, applied, and verified on the Windows 11 domain-joined client.
