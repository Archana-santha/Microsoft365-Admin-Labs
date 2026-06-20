# Microsoft Entra ID: Users, Groups & License Management

## What I Did
Practiced creating and managing cloud-based user identities in Microsoft Entra ID (Azure AD) using a free Developer Tenant. I successfully created multiple test users, organized them into security groups, assigned Microsoft 365 licenses, and verified email functionality through mailbox creation and Outlook access testing.

## Steps Performed

### 1. Accessed Microsoft Entra ID Admin Center
Navigated to the Entra ID admin center at entra.microsoft.com and authenticated with trial account credentials to access identity and access management features.

### 2. Created User Accounts
Used the user creation wizard (Users → New user) to create four test user accounts in the cloud-based directory. Each user received a unique User Principal Name (UPN) and temporary password.

**Users Created:**
- Archana Singh → archana.singh@Archana365Lab.onmicrosoft.com
- David Smith → david.smith@Archana365Lab.onmicrosoft.com
- Emma Wilson → emmawilson@Archana365Lab.onmicrosoft.com
- Richard Smith → richard.smith@Archana365Lab.onmicrosoft.com

**User Account Creation**
![Create user](screenshots/02-create-user-dialog.png)

### 3. Configured User Properties
Edited user profiles to add organizational information including job titles, departments, office locations, and manager relationships. This creates a complete organizational structure and enables automated workflows.

**User Properties Configuration**
![User properties](screenshots/04-user-properties.png)

### 4. Created Security Groups
Used the group creation wizard (Groups → New group) to create security groups for organizing users by function and enabling access control.

**Security Groups Created:**
- IT-Support-Team (for help desk and IT staff)
- Sales-Team (for sales department)

**Group Creation**
![Create group](screenshots/05-create-group-dialog.png)

### 5. Added Members to Groups and Assigned Owners
Populated security groups with user members and designated group owners for management. Owners can add/remove members while regular members access group resources.

**Group Membership Configuration:**

IT-Support-Team:
- Owner: Emma Wilson
- Members: Emma Wilson, Parul Singh

Sales-Team:
- Members: David Smith, Richard Smith

**Group Members View**
![Group members](screenshots/06-group-members.png)

### 6. Assigned Microsoft 365 Licenses
Assigned Microsoft 365 licenses (E1 and E3) to all created users. License assignment automatically triggers mailbox creation and enables access to email, Teams, OneDrive, and other cloud services.

**License Assignment:**
- Archana Singh → Microsoft 365 E3
- David Smith → Microsoft 365 E1
- Emma Wilson → Microsoft 365 E3
- Richard Smith → Microsoft 365 E1
- Parul Singh → Microsoft 365 E3

**After License Assignment - Email IDs Appear**
![Users with licenses](screenshots/08-users-with-licenses.png)

### 7. Tested Email Access
Verified that license assignment successfully created mailboxes and enabled email functionality. Attempted to access Outlook Web (outlook.office.com) with newly created user credentials to confirm end-to-end access.

**Before License:** OwaUserHasNoMailboxAndNoLicenseAssignedException error
**After License:** Successful mailbox creation and Outlook access

**Successful Email Configuration**
![Email access](screenshots/10-outlook-access.png)

### 8. Performed User Management Tasks
Completed common help desk tasks including password resets, account blocking/unblocking, and activity monitoring.

**Password Reset**
![Reset password](screenshots/09-reset-password.png)

**Blocked User Status**
![Blocked user](screenshots/11-blocked-user.png)

**Sign-in Activity Logs**
![Sign-in logs](screenshots/12-sign-in-logs.png)

## Key Learnings

- **Cloud Identity Management:** Entra ID is Microsoft's cloud-based identity service that replaces traditional on-premises Active Directory with internet-accessible identity management.

- **User Principal Name (UPN):** The UPN (firstname.lastname@domain.onmicrosoft.com) is the unique identifier used for sign-in and must be unique within the organization.

- **License-Mailbox Relationship:** License assignment automatically triggers mailbox creation within 5-24 hours. Without a license, a user account exists but has no email access.

- **Security Groups vs. Members:** Security groups organize users for access control. Group owners manage membership while members access shared resources.

- **Group Owners and Members:** Designating group owners enables delegated management without granting full admin rights.

- **License Types:** E1 (basic email and web apps), E3 (desktop applications and advanced features), E5 (premium security and compliance).

- **User Attributes:** Job title, department, manager, and office location enable organizational visibility, org charts, approval workflows, and automated processes.

- **Help Desk Relevance:** User creation, license assignment, group management, and account troubleshooting are core daily help desk responsibilities.

## Real-World Application

In a help desk or IT support role, you would manage scenarios like:

- **Employee Onboarding:** Create user account, assign to appropriate groups, assign license, provision mailbox and services
- **License Management:** Assign E1/E3/E5 based on role, monitor license usage, reclaim licenses from inactive users
- **Group Management:** Create department groups, add new hires to groups, manage access control through group membership
- **Troubleshooting Access:** Diagnose why user cannot access email (missing license), verify group membership, check account status
- **Account Offboarding:** Disable sign-in, remove from groups, reclaim license, archive mailbox before deletion
- **Password Reset:** Handle user-requested password resets, create temporary passwords, enforce security policies

Understanding user and group management is essential for Microsoft 365 support roles.

## Screenshots Summary

| Step | Action | Screenshot |
|---|---|---|
| Create Users | Added users to Entra ID | 02-create-user-dialog.png |
| Configure Users | Set job title, department, manager | 04-user-properties.png |
| Create Groups | Created security groups | 05-create-group-dialog.png |
| Add Members | Populated groups with users | 06-group-members.png |
| Assign Licenses | Assigned E1/E3 licenses to users | 08-users-with-licenses.png |
| Test Email | Verified Outlook access works | 10-outlook-access.png |
| Reset Password | Reset user password | 09-reset-password.png |
| Block User | Disabled user sign-in | 11-blocked-user.png |
| Monitor Activity | Reviewed sign-in logs | 12-sign-in-logs.png |

## Lab Completion Summary

Successfully completed a comprehensive Microsoft Entra ID user and group management lab. Demonstrated practical knowledge of cloud identity management, license administration, group organization, and user account lifecycle management. This lab covers foundational skills required for help desk and IT support roles working with Microsoft 365 environments.

**Difficulty Level:** Beginner to Intermediate  
**Time Required:** 45-60 minutes  
**Key Takeaway:** Licenses drive mailbox creation and service access in cloud identity management
