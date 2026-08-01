# Reviewing the Existing Active Directory Structure

## Purpose

Before creating and applying new Group Policy Objects, the existing Active Directory structure was reviewed to identify the Organizational Units, users, groups, and computers available within the `harper.local` domain.

The Active Directory environment was previously created during an earlier Windows Server and Active Directory lab. Therefore, existing Organizational Units were used instead of creating new ones for this project.

---

## Environment

| Component | Configuration |
|---|---|
| Operating System | Windows Server 2025 |
| Domain | harper.local |
| Directory Service | Active Directory Domain Services |
| Management Tool | Active Directory Users and Computers |

---

## Step 01 — Review Existing Domain Structure

The Active Directory domain was reviewed using Active Directory Users and Computers on the Windows Server 2025 Domain Controller.

The existing domain structure was verified to confirm that the required Organizational Units and domain objects were available before configuring Group Policy.

**Domain Reviewed**


**Screenshot — Active Directory Domain Structure**

![Active Directory Domain Structure](path/to/image.png)

---

## Step 02 — Review Existing Organizational Units

The existing Organizational Units were reviewed to identify where Group Policy Objects could be linked.

The current OU structure includes:

- File Server Groups
- Finance
- HR
- IT
- Servers
- Workstations

Organizational Units are used to organize Active Directory objects and provide a target location for applying Group Policy settings.

**Screenshot — Existing Organizational Units**

![Existing Organizational Units](path/to/image.png)

---

## Step 03 — Review Existing Domain Objects

The existing Active Directory environment was reviewed to confirm the presence of required objects.

The following components were verified:

- Organizational Units
- Domain user accounts
- Security groups
- Windows 11 domain-joined computer

---

## Verification

The Active Directory structure was successfully reviewed using Active Directory Users and Computers.

The following items were confirmed:

- The `harper.local` domain was available
- Existing Organizational Units were visible
- Domain users and groups were organized correctly
- The Windows 11 client was joined to the domain

---

## Result

The existing Active Directory structure was successfully reviewed and confirmed ready for Group Policy configuration.

---

## Skills Demonstrated

- Active Directory administration
- Organizational Unit management
- Domain object organization
- Group Policy targeting
- Windows Server administration
