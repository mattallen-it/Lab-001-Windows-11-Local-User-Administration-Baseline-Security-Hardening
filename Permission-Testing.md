## Permission & Access Testing

###  Test Scenarios

| Scenario | Expected Result | Actual Result |
|--------|----------------|--------------|
| Admin installs software | Allowed | Installation completed successfully without restriction |
| Standard user installs software | Blocked / UAC prompt | Blocked; UAC prompt required administrator credentials |
| Child installs software | Blocked | Installation blocked; no option to elevate privileges |
| Child accesses restricted site | Blocked | Access denied; content filtering enforced |

---

### Analysis & Security Principle

**Outcome Summary:**
- All test results matched expected behavior.
- Privilege boundaries between Administrator, Standard User, and Child accounts were enforced correctly.
- No unauthorized privilege escalation occurred during testing.

**Security Principle Reinforced — Least Privilege:**
- Users were limited to actions appropriate for their assigned role.
- Administrative actions required elevated credentials.
- Child account restrictions reduced exposure to unsafe software and web content.
- This configuration minimizes system risk by preventing unnecessary access.

## Auditing Validation

### Events Logged
- **Event ID 4625**: Failed interactive logon attempt due to invalid credentials.
- **Event ID 4624**: Successful interactive logon using an administrative account.

Both events were recorded in the Windows Security log after enabling logon auditing for success and failure.

### Incident Response Relevance
Logon auditing provides visibility into authentication activity, allowing detection of unauthorized access attempts and confirmation of legitimate logons. Recording both failed and successful events supports investigation, accountability, and timeline reconstruction during security incidents.

