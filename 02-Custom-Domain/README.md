# MS 365 Custom Domain Lab

## What I Did

Practiced adding and configuring a custom domain in Microsoft 365 Admin Center using a free Developer Trial. I set up the domain `Archana365Lab.onmicrosoft.com`, created multiple test users with the domain, configured DNS settings, and verified email functionality by sending and receiving test messages.

---

## Steps Performed

### 1. Accessed Microsoft 365 Admin Center
Navigated to the admin center and located domain management settings under Settings → Domains.

### 2. Added Custom Domain
Used the "Add domain" wizard to add `Archana365Lab.onmicrosoft.com` to the organization. Since this is an onmicrosoft.com domain, Microsoft handles verification and DNS configuration automatically.

**Screenshot 1 - Add Domain Wizard:**
![Add domain](screenshots/03-add-domain-wizard.png)

### 3. Verified Domain Setup
Completed the domain wizard and confirmed the domain status as "Active" and ready for use. No manual DNS configuration was required for the onmicrosoft.com domain.

**Screenshot 2 - Domain Setup Complete:**
![Domain complete](screenshots/05-setup-complete.png)

### 4. Reviewed DNS Records Configuration
Accessed the domain's DNS records page to understand how Microsoft 365 manages mail routing, SPF, DKIM, and DMARC records automatically for onmicrosoft.com domains.

**Screenshot 3 - DNS Records Page:**
![DNS records](screenshots/06-dns-records.png)

### 5. Created Users with Custom Domain
Created three test users in the organization and assigned them email addresses using the new domain:
- Archana S → ArchanaS@Archana365Lab.onmicrosoft.com
- David Smith → david.smith@Archana365Lab.onmicrosoft.com
- Emma Wilson → emmawilson@Archana365Lab.onmicrosoft.com

All users were assigned Microsoft 365 E3 licenses to enable email and other services.

**Screenshot 4 - Active Users with Domain:**
![Active users](screenshots/07-active-users.png)

### 6. Tested Email Functionality
Accessed Outlook Web (outlook.office.com), signed in as one user, and sent a test email to another user on the domain. Verified the email was successfully delivered and received.

**Screenshot 5 - Email Sent:**
![Email sent](screenshots/08-email-sent.png)

**Screenshot 6 - Email Received:**
![Email received](screenshots/09-email-received.png)

---

## Key Learnings

- **Domain Types:** onmicrosoft.com domains are free and included with Microsoft 365; custom purchased domains require separate DNS configuration at a registrar.

- **Automatic DNS Management:** Microsoft 365 automatically manages DNS records (MX, SPF, DKIM, DMARC) for onmicrosoft.com domains, requiring no manual setup.

- **User-Domain Relationship:** Every user must be assigned to a domain; their email address and User Principal Name (UPN) are derived from the domain.

- **License Requirement:** Users need an active license (E3 or higher) to access email, Teams, OneDrive, and other services.

- **Email Verification:** Email delivery between users on the same domain confirms proper domain configuration and mail routing.

- **Professional Email Setup:** Domains provide professional email addresses and enable organizations to structure their email infrastructure.

- **Help Desk Context:** Help desk teams frequently manage domain-related tasks including user creation, license assignment, and troubleshooting email delivery issues.

---

## Real-World Application

In a help desk role, you would encounter scenarios like:
- **New Employee Onboarding:** Create user account, assign to company domain, set up email
- **Email Delivery Issues:** Verify domain DNS configuration when users report delivery problems
- **Account Management:** Create, modify, or disable user accounts associated with specific domains
- **Domain Troubleshooting:** Diagnose issues when emails aren't sending or are marked as spam

Understanding domain configuration is foundational for supporting Microsoft 365 users.

---

## Lab Summary

Successfully completed a hands-on Microsoft 365 domain configuration lab covering domain setup, user creation with domain email addresses, DNS understanding, and email testing. This demonstrates practical knowledge applicable to help desk support roles.

**Difficulty Level:** Beginner to Intermediate  
**Key Takeaway:** Domains are the organizational structure that enable email and services in Microsoft 365

---

## Additional Resources

- LAB-NOTES.md - Detailed technical notes and concepts
- DNS-RECORDS-REFERENCE.md - Complete DNS records guide for custom domains
- GITHUB-STRUCTURE-GUIDE.md - Repository organization details
