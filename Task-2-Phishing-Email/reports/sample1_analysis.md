# Phishing Email Investigation Report - Sample 1

## Report Information

| Field | Details |
|-------|---------|
| Report Title | Fake Assessment Report Email Analysis |
| Analyst | Prasiddha Pal |
| Date | 01 July 2026 |
| Category | Phishing / Credential Harvesting |
| Severity | High |

---

# Objective

The objective of this investigation is to analyze a phishing email that impersonates an organization's Human Resources (HR) department. The email attempts to trick recipients into clicking a malicious hyperlink disguised as an employee assessment report, potentially leading to credential theft.

---

# Sample Overview

This phishing email masquerades as an official HR communication informing employees that their annual performance assessment report is available for review. The recipient is instructed to click a link labeled **"Open My Assessment Report"**.

This type of phishing attack relies on employee trust in HR communications and exploits curiosity regarding performance reviews.

---

# Email Information

| Field | Value |
|--------|-------|
| Subject | Please Review Your 2025 Assessment Report |
| Sender | Cynthia Burns `<cburns13@gapps.bcsds.org>` |
| Recipient | Hidden |
| Email Type | Employee Assessment Notification |
| Attack Type | Credential Harvesting |

---

# Initial Observation

At first glance, the email appears professional.

It contains:

- Professional formatting
- Formal language
- HR department signature
- Legitimate-looking assessment notification

These characteristics are intended to reduce suspicion and encourage the recipient to trust the message.

---

# Sender Analysis

The sender claims to represent the Human Resources department.

However, before trusting the email, users should verify:

- Whether the sender is an actual HR employee.
- Whether the email domain belongs to the organization.
- Whether the email was expected.

A phishing attacker often impersonates internal employees or departments to increase credibility.

**Finding**

⚠ Sender identity should be verified before interacting with the email.

---

# Subject Analysis

**Subject**

```
Please Review Your 2025 Assessment Report
```

### Observation

The subject line creates curiosity because employees commonly expect annual performance evaluations.

Attackers frequently use HR-related subjects because recipients are more likely to open such emails.

**Finding**

Medium Risk

---

# Email Body Analysis

The email states that:

- The assessment report has been shared.
- Employees should review it.
- A form must be completed.
- The report should be reviewed today.

Instead of attaching the report directly, the email asks the recipient to click a hyperlink.

This behavior is commonly observed in credential harvesting attacks.

**Finding**

The embedded hyperlink is the primary phishing indicator.

---

# Hyperlink Analysis

Displayed link:

```
Open My Assessment Report
```

The actual destination should always be verified before clicking.

Security analysts recommend:

- Hovering over hyperlinks.
- Checking the URL.
- Scanning the URL using VirusTotal or URLScan.

**Risk**

High

---

# Social Engineering Analysis

The attacker employs several psychological manipulation techniques.

| Technique | Used |
|-----------|------|
| Authority | ✅ |
| Trust | ✅ |
| Curiosity | ✅ |
| Urgency | ✅ |
| Fear | ❌ |
| Financial Reward | ❌ |

### Explanation

The attacker impersonates the HR department, a trusted authority within the organization.

Employees are naturally curious about performance reviews, making them more likely to click the provided link.

---

# Phishing Indicators Identified

| Indicator | Status |
|-----------|--------|
| HR Impersonation | ✅ |
| Credential Harvesting Attempt | ✅ |
| Suspicious Hyperlink | ✅ |
| Social Engineering | ✅ |
| Unexpected Email | ✅ |
| Sense of Urgency | ✅ |

---

# Potential Impact

If the victim clicks the malicious link and enters credentials, attackers may obtain:

- Employee username
- Password
- Corporate email account access
- Sensitive organizational information

Possible consequences include:

- Account Takeover
- Identity Theft
- Business Email Compromise (BEC)
- Data Breach

---

# Risk Assessment

| Category | Level |
|----------|-------|
| Likelihood | High |
| Impact | High |
| Overall Severity | High |

---

# Recommendations

- Verify emails claiming to be from HR before responding.
- Hover over hyperlinks before clicking.
- Access employee portals by typing the official website manually.
- Never enter credentials after clicking links received through unsolicited emails.
- Enable Multi-Factor Authentication (MFA).
- Report suspicious emails to the organization's IT or Security team.
- Keep endpoint protection software updated.

---

# MITRE ATT&CK Mapping

| Technique | ID |
|-----------|----|
| Phishing | T1566 |
| Spearphishing Link | T1566.002 |
| Credential Phishing | T1566 |

---

# Conclusion

This email demonstrates multiple phishing characteristics, including HR impersonation, social engineering, and the use of a hyperlink likely intended to redirect victims to a fraudulent login page.

Although the email appears professional, its reliance on an embedded link instead of providing the report directly is a strong indicator of a credential harvesting attack.

Users should verify the legitimacy of similar emails before interacting with any links or submitting sensitive information.

---

# References

- UC Berkeley Information Security Office – Phish Tank Archive
- MITRE ATT&CK Framework
- CISA – Recognizing and Avoiding Phishing Scams
