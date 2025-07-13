# 📧 Email Phishing Analysis

## 🎯 Objective

The **Email Phishing Analysis** project simulates how a Security Analyst investigates a real phishing email. This includes examining email headers, inspecting return paths, checking sender domains, verifying SPF records, and analyzing the email using online threat intelligence platforms. It also involves testing how an email security solution like **Bitdefender** detects malicious payloads.

---

## 🧠 Skills Learned

- Email header analysis and interpretation
- SPF, DKIM, and Return-Path validation
- Threat intelligence lookups (AbuseIPDB, URLScan, Symantec Threat Intelligence)
- Email filtering and security configuration using **Bitdefender Email Protection**
- Incident response actions after phishing detection
- Real-world scenario testing using GitHub-sourced phishing samples

---

## 🧰 Tools & Platforms Used

- 🛡️ **Bitdefender Email Security** – email filtering, real-time protection
- 🔍 **Symantec Threat Intelligence** – threat reputation analysis
- 🔗 **URLScan.io** – URL behavior scanning
- 🌐 **AbuseIPDB** – malicious IP reputation checks
- 📬 **GitHub (PhishingPot)** – real phishing email samples
- 🧠 **SPF/DKIM/DMARC Validators** – email authenticity checks

---

## 📂 Project Steps

### 1️⃣ Configure Bitdefender Email Protection
- Created and added a new email account under Bitdefender
- Enabled scanning and protection rules
- Verified real-time email scanning was active

### 2️⃣ Import a Real Phishing Email
- Sourced a phishing sample from [PhishingPot GitHub](https://github.com/PhishingPot/phishing-pot)
- Sent the phishing email to the protected email inbox

### 3️⃣ Analyze the Email
- **Header Analysis**:
  - Checked the *Return-Path*, *Received-SPF*, and *Sender IP*
  - Identified mismatches and potential spoofing

- **Reputation Check**:
  - Analyzed suspicious links with **URLScan.io**
  - Verified sender IP reputation using **AbuseIPDB**
  - Cross-checked domain using **Symantec Threat Lookup**

### 4️⃣ Bitdefender Detection
- The phishing email was **flagged as dangerous**
- Alert was triggered immediately, demonstrating working protection

### 5️⃣ Response Plan

| Action                          | Description                                                  |
|-------------------------------|--------------------------------------------------------------|
| 🧹 Delete from mailbox         | Remove malicious emails from the user inbox                 |
| 🔁 Check for other victims     | Determine if other employees received similar messages      |
| ❗ Ensure no links were clicked | Interview/report from affected users                        |
| 🔐 Password reset              | Reset credentials if links were clicked or data entered     |
| 👀 Investigate lateral spread | Look for signs of internal compromise or beaconing activity |

---

## 📌 Summary

This project replicates a real-world phishing investigation handled by Tier 1 SOC Analysts. From threat detection to incident response, it demonstrates the analyst’s role in keeping users safe from credential harvesting attacks and email-borne threats.

---

## 🧑‍💻 Author

**Dipak Pakhrin**  
