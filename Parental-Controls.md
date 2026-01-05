# Parental-Controls

**Lab:** Windows 11 Multi-User Administration  
**Section:** Child Account — Parental Controls  
**Platform:** Windows 11 Pro

---

## 1) Purpose
Parental controls were configured to enforce age-appropriate access, restrict unsafe content and applications, limit screen time, and require permission for purchases. These settings mirror access control and policy enforcement practices used in shared or restricted user environments.

---

## 2) Account Scope
- **Account type:** Child (Standard user)  
- **Management platform:** Microsoft Family Safety  
- **Admin role:** Local administrator responsible for configuration and validation  
- **Policy scope:** Settings apply across all activities of the child account  

---

## 3) Screen Time Configuration
**Status:** Enabled  
**Scope:** Windows device  

| Day        | Time Limit | Available Hours     |
|------------|------------|---------------------|
| Sunday     | 2 hours    | 07:00 AM – 08:00 PM |
| Monday     | 1 hour     | 07:00 AM – 08:00 PM |
| Tuesday    | 1 hour     | 07:00 AM – 08:00 PM |
| Wednesday  | 1 hour     | 07:00 AM – 08:00 PM |
| Thursday   | 1 hour     | 07:00 AM – 08:00 PM |
| Friday     | 1 hour     | 07:00 AM – 08:00 PM |
| Saturday   | 2 hours    | 07:00 AM – 08:00 PM |

**Behavior:**
- Device access is restricted to defined time windows.
- Once the daily limit is reached, further usage is blocked.

---

## 4) Content & Safety Controls

### 4.1 Age Rating
- **Setting:** Age limit for apps, games, and media  
- **Configured value:** 8  

**Effect:** Filters out age-inappropriate content and media.

---

### 4.2 Web Safety
- **Setting:** Web and search filtering  
- **Configured value:** Enabled  

**Details:**
- Unsafe browsers and mature content are blocked.
- SafeSearch is enforced on Bing.
- Only approved browsers (e.g., Microsoft Edge) are permitted.

**Purpose:** Reduces exposure to inappropriate online content.

---

## 5) Purchase & Permission Controls

### 5.1 Ask to Buy
- **Setting:** Purchase approval  
- **Configured value:** Enabled  

**Behavior:**
- Requires organizer permission for all purchases.

**Purpose:** Prevents unauthorized purchases.

---

## 6) Activity Reporting & Notifications

### 6.1 Weekly Email Report
- **Setting:** Weekly activity summary  
- **Configured value:** Enabled  

**Behavior:**
- Weekly activity usage reports are sent to organizers and the child account.

### 6.2 On-Demand Activity Email
- **Setting:** Activity reporting via email  
- **Configured value:** Enabled  

---

## 7) Apps & Games Restrictions

### 7.1 Enforcement Model
Application access is restricted by explicitly blocking all non-approved applications.

### 7.2 Allowed Applications
- **Microsoft Edge** — filtered web browsing  
- **Roblox game client** — permitted game  

### 7.3 Blocked Applications
All non-approved applications are explicitly blocked, including system apps, productivity tools, and the Microsoft Store. This prevents unapproved software usage and new application installations.

### 7.4 Risk Mitigation
Permitted applications are further controlled through age rating enforcement, screen time limits, purchase approval, and activity reporting.

---

## 8) Validation
- **Screen Time:** Verified daily limits and availability windows.  
- **Web Safety:** Confirmed unsafe content filtering and SafeSearch enforcement.  
- **Apps & Games:**
  - Edge and Roblox launch successfully under the child account.
  - All other applications display a blocked status.
  - Microsoft Store access is blocked, preventing new installs.

---

## 9) Issues / Notes
- Microsoft Family Safety does not provide a single allow-only toggle; allow-listing is achieved through explicit blocking of non-approved applications.

---

## 10) Final Status
Parental controls were successfully configured to enforce age-appropriate access, content filtering, screen time limits, purchase approval, and application restrictions for the child account.

**Status:** ✅ Completed  
**Last updated:** 2026-01-05
