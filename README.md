# Task-2

# 📧 Phishing Email Analysis: CEO Impersonation Attempt

## 🔍 Objective
This task involves analyzing a real-world-style phishing email aimed at impersonating a CEO to manipulate a CFO into processing an unauthorized financial transaction. The goal is to detect and document the key indicators of a phishing attempt using a structured, step-by-step methodology.

---

## 🧪 Email Sample Overview

**Sender Display Name:** John Brownstown (CEO Hi-Tech)  
**Sender Email:** jbrownstown@hi-tech-c0rp.test  
**Recipient:** Alice Underwood (CFO Hi-Tech)  
**Subject:** Important Bank Payment Instructions  
**Date:** April 15, 2023

---

## ✅ Step-by-Step Analysis

### 1. **Examine Sender's Email Address**
-  Uses a **typosquatted domain** (`hi-tech-c0rp.test`) instead of the official one (`hi-tech-corp.com`).
-  `.test` domain is invalid for business use.
-  Likely spoofed or impersonated.

### 2. **Check Email Headers**
- Suggests discrepancy in `Return-Path`, `Reply-To`, and originating IP.
- SPF, DKIM, and DMARC validations are likely to **fail** or be **missing**.

### 3. **Look for Suspicious Links or Attachments**
- Mentions “enclosed vendor banking information” with **no visible attachment**.
- May be a setup for a follow-up phishing or malware email.

### 4. **Urgent or Threatening Language**
- "ASAP", "within the next hours", "before the end of the day" used to pressure action.

### 5. **Mismatched URLs**
- No visible URLs in this message, but such phishing emails typically hide malicious links behind legitimate-looking text.

### 6. **Spelling and Grammar Errors**
- Awkward phrasing: “vendor banking information instructions”, “within the next hours”.
- Unnatural sentence flow and lack of professional tone.

---

##  Summary of Phishing Traits Found

| Trait | Description |
|-------|-------------|
| **Typosquatted Domain** | hi-tech-**c0**rp.test instead of hi-tech-**co**rp.com |
| **Urgency** | Repeated use of time pressure to rush decision-making |
| **Lack of Verification** | No additional documentation or secondary approval |
| **Impersonation of Executive** | Pretending to be the CEO to influence the CFO |
| **Language Issues** | Grammar errors, awkward wording, unprofessional closing |
| **No Digital Signature** | No email footer or company branding |

---

##  Verdict

>  **Phishing Attempt Detected (Business Email Compromise)**  
> This email attempts to manipulate a financial officer into transferring money through impersonation and psychological pressure. It must be reported, blocked, and added to training datasets.

---

## Files Included

- `phishing-email-example.webp`: Screenshot of the suspicious email
- `README.md`: This documentation file

---

## 🛡️ Recommended Action

- Block the domain `hi-tech-c0rp.test`
- Report to security team for awareness
- Use as a case study for employee phishing training

---

## 📚 References

- [MxToolbox Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)

