# Local Security Policy Configuration

## Objective
Apply and document local password and account lockout policies on a Windows 11 Pro system to reduce brute-force and credential abuse risk in a multi-user environment.

## Password Policy
- Password complexity: Enabled
- Minimum password length: 12 characters
- Enforce password history: 10 passwords
- Maximum password age: 999 days
- Store passwords using reversible encryption: Disabled

## Account Lockout Policy
- Account lockout threshold: 5 invalid attempts
- Account lockout duration: 15 minutes
- Reset lockout counter after: 15 minutes
- Allow administrator account lockout: Disabled

## Rationale
- Long, complex passwords reduce guessing and credential stuffing risk.
- Password history prevents immediate reuse.
- Lockout policies limit online brute-force attempts.
- Administrator lockout disabled to prevent accidental denial of service.
- Forced rotation avoided in favor of strong passwords unless compromise occurs.

## Validation
- Verified settings in Local Security Policy (`secpol.msc`).
- Screenshots captured for password and account lockout policies.

## Evidence

### Password Policy
![Password Policy Configuration](evidence/password-policy.png)

### Account Lockout Policy
![Account Lockout Policy Configuration](evidence/account-lockout-policy.png)


