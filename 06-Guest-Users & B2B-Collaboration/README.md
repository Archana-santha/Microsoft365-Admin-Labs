# Microsoft 365: Guest Users & B2B Collaboration

## What I Did
Practiced guest user management and B2B collaboration in Microsoft 365 using a free Developer Tenant. I successfully invited external users as guests to Teams and SharePoint, managed guest permissions, reviewed B2B direct connect capabilities, and documented real-world collaboration scenarios. This lab demonstrates understanding of external user access management and modern organization collaboration patterns.

## Steps Performed

### 1. Accessed Guest Users Management
Navigated to Microsoft 365 Admin Center to understand guest user administration. Reviewed the guest user management interface and existing guest configurations. This shows where IT professionals manage external user access.

**Guest Users Interface**
![Guest users list](screenshots/01-guest-users-list.png)

### 2. Reviewed Guest Access Settings
Checked organizational settings for guest collaboration policies. Verified settings that control who can invite guests and what permissions guests receive. Understanding these settings is critical for security and compliance.

**Guest Access Settings:**
```
Current Settings:
├─ Users can invite guests: Enabled
├─ Guest permissions level: Configured
├─ Collaboration restrictions: In place
└─ External sharing: Managed
```

**Screenshot 2:** Guest access settings
![Guest access settings](screenshots/02-guest-access-settings.png)

### 3. Invited Guest to IT Support Team
Successfully invited external user (contractor@externalcompany.com) as a guest to the IT Support Team in Microsoft Teams. This demonstrates how organizations enable contractors and partners to collaborate on specific projects while maintaining security boundaries.

**Invitation Process:**
- Guest email provided
- Guest role assigned (not full member)
- Invitation sent to external user
- Guest gains access to team and channels

**Guest Invited to Team**
![Guest invited to team](screenshots/03-invite-guest-team.png)

### 4. Attempted Guest SharePoint Access
Tried to invite external user (partner@example.com) to SharePoint site for document collaboration. Encountered B2B collaboration restriction error, which revealed actual tenant configuration limitations.

**SharePoint Sharing Process:**
- Navigated to SharePoint site
- Used Share function
- Entered partner email
- Encountered B2B configuration error

**Screenshot 4:** B2B Collaboration Error
![B2B configuration error](screenshots/04-b2b-sharepoint-error.png)

### 5. Investigated B2B Configuration
Reviewed External Identities settings in Entra ID to understand B2B collaboration configuration. Checked External Collaboration Settings and Cross-tenant Access Settings to identify configuration restrictions.

**Configuration Discovery:**
```
External Collaboration Settings:
├─ Guest invite restrictions: Anyone can invite
└─ Settings appear enabled

Cross-tenant Access Settings:
├─ B2B collaboration: Allowed
├─ B2B direct connect: Blocked (explanation for error)
└─ Conflicting configuration identified
```

**Screenshot 5:** External Collaboration Settings
![External collaboration settings](screenshots/05-external-identities.png)

### 6. Reviewed Guest User Admin Status
Accessed Guest Users page in Admin Center to verify guest account creation and status. The external user (contractor) appears in the tenant as a guest with #EXT# suffix in their email address, indicating external user status.

**Guest User Confirmation:**
- Display name: contractor
- Email: contractor_externalcompany.com#EXT#@Archana365Lab.onmicrosoft.com
- User type: Guest (indicated by #EXT# suffix)
- Status: Active in organization

**Screenshot 6:** Guest User Details
![Guest user details](screenshots/06-guest-details.png)

### 7. Managed Guest Team Membership
Accessed IT Support Team members list to verify guest was added to team and demonstrated how to manage guest permissions. Showed guest displayed with "Guest" role indicator and removal option (X button).

**Guest Management:**
- Guest appears in team members list
- Role shown as "Guest" in Team role column
- Removal option available via X button
- Can modify permissions if needed

**Screenshot 7:** Guest Team Management
![Guest team management](screenshots/07-guest-management.png)

### 8. Understood B2B Direct Connect
Reviewed B2B Direct Connect capabilities for seamless cross-organizational collaboration. This modern approach allows teams from different organizations to collaborate without traditional guest invitations.

**B2B Direct Connect Features:**
```
What it enables:
├─ External teams join your shared channels
├─ Seamless collaboration experience
├─ Maintains organizational identity
├─ Cleaner access management
└─ Better for partner companies
```

**B2B Direct Connect Capability**
![B2B Direct Connect](screenshots/08-b2b-direct-connect.png)

### 9. Documented Real-World Scenarios
Created documentation of practical guest user scenarios that organizations use daily. These demonstrate value of guest access management for business collaboration.

**Real-World Scenarios Documented:**

**Scenario 1: Contractor Access**
- Hire 6-month contractor for project
- Invite as guest to project team
- Grant edit access to project files
- Limit visibility to that project only
- Remove when contract ends
- Clean offboarding process

**Scenario 2: Partner Collaboration**
- Partner company needs to collaborate
- Invite partner staff as guests
- Provide Teams and SharePoint access
- Maintain security boundary
- Time-limited access for project duration

**Scenario 3: Client Project Visibility**
- Client needs project visibility
- Invite client rep as guest
- View-only access to team
- Can see progress and deliverables
- Cannot see budget or sensitive data
- Remove after project completion

**Screenshot 9:** Real-World Scenarios
![Real-world scenarios](screenshots/09-scenarios.png)

### 10. Documented Help Desk Support Scenarios
Created troubleshooting guide for help desk support of guest users. This represents common tickets help desk handles regarding guest access.

**Common Help Desk Tickets:**

**Ticket: "I can't access the team"**
- Check if guest is added to team
- Verify invitation was accepted
- Check permissions level
- Resync if needed
- Add guest if missing

**Ticket: "Guest user can't see files"**
- Verify guest added to SharePoint
- Check sharing permissions
- Confirm permission level (Edit/View)
- Wait for sync (30 min normal)
- Retry access

**Ticket: "How do I invite external user?"**
- Go to team members
- Click add member
- Enter external email
- Select Guest role
- Send invitation

**Screenshot 10:** Help Desk Support Guide
![Help desk support](screenshots/10-helpdesk-support.png)

## Key Learnings

- **Guest Users:** External people with limited access to specific resources. Identified by #EXT# suffix in their email address. Critical for contractors, partners, and temporary collaborators.

- **Guest Roles:** Can be assigned as Owner, Member, or Guest. Most common is Member or Guest. Controls what guests can do in teams and channels.

- **B2B Collaboration:** Business-to-Business collaboration allowing external users to access your organization's resources. Requires proper configuration to enable.

- **B2B Direct Connect:** Modern approach for partner organizations to collaborate in shared channels without traditional guest invitations. More seamless experience.

- **Guest Invitation Process:** External user receives email invitation, accepts to create account, then gains access. Synchronized with organization's identity system.

- **SharePoint Sharing:** Files can be shared directly with guests. Requires both B2B collaboration settings and SharePoint sharing policies enabled.

- **Tenant Configuration:** B2B features require proper configuration in External Identities settings. Cross-tenant access settings control what external organizations can access.

- **Help Desk Relevance:** Common tickets include: "Add me to team," "I can't access files," "Invite external user," "Remove guest access." Requires understanding of guest lifecycle.

- **Security Boundaries:** Guests have limited access to organization. Cannot see full directory, only invited resources. Maintains security while enabling collaboration.

- **Guest Lifecycle:** From invitation through active collaboration to removal. Clean offboarding is important for security and compliance.

## Real-World Application

In an IT administration or help desk role, you would manage scenarios like:

- **Contractor Onboarding:** Hire contractor for 3-month project. Add to project team. Grant file access. Remove when contract ends. Process is repeated many times.

- **Partner Collaboration:** Work with technology partner on integration project. Invite their team members as guests. Collaborate on deliverables. Clean removal after project.

- **Customer Advisory Board:** Hold quarterly meetings with customer representatives. Invite attendees as guests. Share product roadmap. Archive team after meeting.

- **Vendor Access:** Vendor needs to access specific SharePoint documents. Share site with vendor contacts. Limit to read-only access. Remove after contract.

- **Guest Access Troubleshooting:** User calls: "I can't access the team." Help desk checks if they're added. Adds if missing. Verifies permissions. Resolves in 5 minutes.

- **B2B Configuration Issues:** Organization can't share with external partners. IT team checks B2B settings. Enables cross-tenant access. Partners can now collaborate.

- **Security Review:** Annual review of active guest users. Remove inactive guests. Verify appropriate access levels. Ensure no excessive permissions.

- **Compliance Reporting:** Generate report of guest users and access. Document business reasons for each guest. Maintain audit trail for compliance.

Understanding guest user management is essential as most modern organizations work with external partners, contractors, and clients. Help desk handles guest-related requests daily.

## Screenshots Summary

| Step | Action | Screenshot |
|---|---|---|
| 1 | Accessed guest management | 01-guest-users-list.png |
| 2 | Reviewed guest settings | 02-guest-access-settings.png |
| 3 | Invited guest to team | 03-invite-guest-team.png |
| 4 | Attempted SharePoint sharing | 04-b2b-sharepoint-error.png |
| 5 | Reviewed configuration | 05-external-identities.png |
| 6 | Checked guest status | 06-guest-details.png |
| 7 | Managed team membership | 07-guest-management.png |
| 8 | B2B Direct Connect | 08-b2b-direct-connect.png |
| 9 | Real-world scenarios | 09-scenarios.png |
| 10 | Help desk support | 10-helpdesk-support.png |

## Lab Completion Summary

Successfully completed an intermediate Microsoft 365 Guest Users & B2B Collaboration lab covering guest user creation, access management, team and SharePoint sharing, B2B configuration, and real-world scenarios. Demonstrated understanding of external user access models, collaboration patterns, and common help desk support issues. This lab covers essential skills as most organizations work with external users and require help desk support for guest management.

**Difficulty Level:** Intermediate  
**Time Required:** 90 minutes  
**Key Takeaway:** Guest user management enables secure external collaboration by providing limited access to specific resources while maintaining organizational security boundaries
