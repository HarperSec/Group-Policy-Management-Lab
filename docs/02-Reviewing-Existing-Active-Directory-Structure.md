# Reviewing the Existing Active Directory Structure

## Overview

Before creating and applying new Group Policy Objects, the existing Active Directory structure was reviewed to identify the Organizational Units, users, groups, and computers available in the domain.

The Active Directory environment was previously configured as part of an earlier Windows Server and Active Directory lab. Therefore, new Organizational Units were not created for this project.

## Existing Domain

The Active Directory domain used in this lab is:

`harper.local`

The domain is hosted on a Windows Server 2025 Domain Controller.

## Existing Organizational Units

The existing Organizational Units were reviewed in Active Directory Users and Computers.

The Organizational Units in the environment are used to organize domain objects and provide a structure for applying Group Policy settings to specific users or computers.

File Server Groups  
Finance  
HR  
IT  
Servers  
Workstations  

## Screenshots  
### Existing OUs
[![Existing OUs](path/to/image.png)](https://github.com/HarperSec/Group-Policy-Management-Lab/blob/main/screenshots/01-Active-Directory-Organizational-Units.png)

## Purpose of Organizational Units

Organizational Units allow administrators to organize users, groups, and computers based on departments, roles, locations, or administrative requirements.

OUs can also be used to target Group Policy Objects. When a GPO is linked to an OU, the policy can apply to the users and computers located within that OU.

## Existing Domain Objects

The environment already contains the following Active Directory components:

* Organizational Units
* Domain user accounts
* Security groups
* A Windows 11 domain-joined computer
* Existing domain security settings

## Verification

The existing Active Directory structure was reviewed using **Active Directory Users and Computers** on the Windows Server 2025 Domain Controller.

The following items were verified:

* The `harper.local` domain was available
* Existing Organizational Units were visible
* Domain users were located in the appropriate OUs
* Security groups were available
* The Windows 11 client was joined to the domain

## Result

The existing Active Directory structure was successfully reviewed and was ready for Group Policy configuration.

## Skills Demonstrated

* Active Directory administration
* Organizational Unit management
* Domain object organization
* Group Policy targeting
* Windows Server administration
