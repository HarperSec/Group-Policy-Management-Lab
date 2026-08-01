# Reviewing the Existing Active Directory Environment

## Purpose

Before configuring Group Policy Objects (GPOs), the existing Active Directory environment was reviewed to confirm that the required Organizational Units (OUs), users, groups, and computers were available within the `harper.local` domain.

The Active Directory structure was created during the previous Windows Server Active Directory Home Lab. The existing OU design was reused for Group Policy testing instead of creating new organizational structures.

---

## Environment

| Component | Configuration |
|---|---|
| Operating System | Windows Server 2025 |
| Domain | `harper.local` |
| Directory Service | Active Directory Domain Services |
| Management Tool | Active Directory Users and Computers |

---

# Reviewing the Existing Domain Structure

Active Directory Users and Computers was opened on the Windows Server 2025 Domain Controller to review the current `harper.local` domain structure.

The domain was checked to confirm that the existing Organizational Units and domain objects were available before configuring Group Policy.

![Active Directory Domain Structure](path/to/image.png)

---

# Reviewing Organizational Units Used for Group Policy

The existing Organizational Units were reviewed to identify where Group Policy Objects would be linked.

The current OU structure includes:

- File Server Groups
- Finance
- HR
- IT
- Servers
- Workstations

These Organizational Units provide separate locations for applying Group Policy settings to specific users, computers, and departments.

![Existing Organizational Units](path/to/image.png)

---

# Reviewing Existing Domain Objects

The Active Directory environment was reviewed to confirm that required objects were available for Group Policy testing.

The following objects were verified:

- User accounts
- Security groups
- Organizational Units
- Domain-joined Windows 11 workstation

The existing objects will be used as targets when creating and applying Group Policy configurations.

---

## Result

The existing Active Directory environment was confirmed to be ready for Group Policy configuration.

The current OU structure from the Active Directory Home Lab will be used throughout this project to create, link, and test Group Policy Objects.

---

## Skills Demonstrated

- Active Directory administration
- Organizational Unit management
- Domain object organization
- Group Policy planning
- Windows Server 2025 administration
