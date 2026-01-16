# lab 001 – windows 11 local user administration & baseline security hardening

## What This Lab Is
A practical Windows 11 Pro lab that simulates real Tier 1 IT support and entry-level security tasks.  
The lab focuses on configuring local user accounts, enforcing least privilege, and basic auditing.  
All actions are documented as internal IT notes rather than a tutorial.

## Environment
- **Operating System:** Windows 11 Pro
- **System Type:** Standalone local system (no domain)
- **Accounts Configured:**
  - Local Administrator account
  - Standard User account
  - Child / Restricted User account
- **Tools Used:**
  - Local Users and Groups
  - Local Security Policy (`secpol.msc`)
  - Event Viewer

## Repository Structure

- README.md — Lab overview, scope, and security concepts
- Lab-Objective.md — Purpose and framing of the lab
- Account-Setup.md — Account creation and administrator actions
- Local-Security-Policy.md — Password, lockout, and auditing policy configuration
- Permission-Testing.md — Validation of access controls across user roles
- Parental-Controls.md — Child account restrictions and testing
- Lessons-Learned.md — Reflections and takeaways from the lab
- evidence/ — Supporting screenshots for security policy configuration


## Skills Demonstrated
- Local user account creation and management
- Role-based access control using local accounts
- Enforcement of least privilege
- Permission testing across multiple user roles
- Enabling and verifying security auditing
- Clear, structured technical documentation

## Security Concepts Applied
- Least Privilege
- Account Separation
- Auditing and Accountability
- Basic Incident Response Readiness

This lab intentionally focuses on local account administration and security controls and does not include Active Directory, Group Policy, or enterprise tooling.

