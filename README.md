# Group Policy Management Lab

## Overview

This project demonstrates the use of Group Policy Objects (GPOs) to centrally manage and configure users and computers in an Active Directory domain environment.

The lab builds on an existing Windows Server 2025 Active Directory environment containing Organizational Units (OUs), domain users, security groups, a domain password policy, and a Windows 11 domain-joined client.

The purpose of this project is to demonstrate how Group Policy can be created, configured, linked, applied, and tested within a Windows domain environment.

## Lab Objectives

* Review the existing Active Directory Organizational Unit structure
* Create and configure new Group Policy Objects
* Link GPOs to existing Organizational Units
* Apply user and computer configuration settings
* Update Group Policy on a Windows 11 client
* Verify that Group Policy settings are applied successfully
* Troubleshoot Group Policy application issues

## Lab Environment

| Component               | Configuration                          |  

| Server Operating System | Windows Server 2025                    |  
| Server Role             | Active Directory Domain Controller     |  
| Active Directory Domain | `harper.local`                         |  
| Client Operating System | Windows 11                             |  
| Client Status           | Joined to the `harper.local` domain    |  
| Management Tool         | Group Policy Management Console (GPMC) |

## Existing Configuration

The following components were configured before beginning this project:

* Active Directory Domain Services
* Active Directory Organizational Units
* Domain users and security groups
* A domain password policy
* A Windows 11 domain-joined client
* Department file shares
* NTFS permissions
* Share permissions

## Group Policy Configurations

The following policies will be configured and tested during this lab:

* Interactive logon message
* User-based access restriction
* Additional Group Policy settings as applicable

## Skills Demonstrated

* Active Directory administration
* Group Policy administration
* Group Policy Object creation
* GPO linking and configuration
* Windows client management
* Policy testing and verification
* Windows troubleshooting
* Technical documentation

## Repository Structure

```text
Group-Policy-Management-Lab/
│
├── README.md
│
├── docs/
│   ├── 01-Group-Policy-Overview.md
│   ├── 02-Reviewing-Existing-Active-Directory-Structure.md
│   ├── 03-Creating-and-Configuring-a-GPO.md
│   ├── 04-Linking-and-Applying-the-GPO.md
│   └── 05-Troubleshooting.md
