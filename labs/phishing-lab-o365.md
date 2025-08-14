<!-- Ryvora Lab: Microsoft 365 Phishing Investigation -->
<!-- Animated README for Student Portfolio -->

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?size=26&color=00FF99&center=true&vCenter=true&width=850&lines=Microsoft+365+Phishing+Investigation;Hands-On+SOC+Analysis;Documented+Findings+%26+Workflow" alt="Lab Banner">
</p>

---

## 🧑‍💻 Incident Report — Microsoft 365 Phishing Investigation

**Role:** SOC Analyst (Ryvora Training Environment)  
**Platform:** Windows VM via Guacamole  
**Tools Used:**  
- Microsoft 365 Security & Compliance Center  
- Outlook Web Access  
- Exchange Message Trace  
- Microsoft Defender for Office 365  

---
###  Initial Investigation
Upon accessing **Microsoft 365 Security & Compliance**, we navigated to **Email & Collaboration Security** to review recent inbound mail.  
The target account, **Accounting@Ryvora.onmicrosoft.com**, was reported to have received a suspicious external email.

**Timeframe of Interest:**  
> August 8, 2025 — between **10:40 PM and 11:20 PM** (based on incident briefing)

---

### Message Trace Analysis
Ran a **Message Trace** query for all inbound emails to the Accounting mailbox within the given time window.


---

### 6Indicators of Compromise (IOCs)

| Type | Value |
|------|-------|
| Sender Email | billing.info@zohomail.com |
| Sender IP | 203.0.113.45 |
| Malicious URL | hxxps://secure-login-verification[.]com |
| File Hash (MD5) | 5d41402abc4b2a76b9719d911017c592 |

---

### Phishing Bypass Technique
The attacker bypassed basic filters by:
- Registering a **lookalike domain**
- Sending during **off-hours**
- Using an HTML attachment instead of embedding malicious content directly in the email body

---

### Lessons Learned
This lab reinforced my ability to:
- Use **Message Trace** for targeted email searches
- Perform **email header analysis** to validate sender authenticity
- Leverage **Defender logs** for phishing detection
- Document IOCs for incident reporting
- Understand the role of **SPF, DKIM, and DMARC** in phishing prevention

---

### 🏁 Final Summary
This was a simulated **real-world SOC phishing investigation** where I:
1. Accessed a live VM environment  
2. Queried and isolated suspicious emails  
3. Verified authenticity via email header forensics  
4. Leveraged Microsoft Defender for deeper inspection  
5. Documented all findings in a structured incident report format

---

<p align="center">
  <img src="https://img.shields.io/badge/Hands--On%20Skills-Email%20Forensics-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Skills-Microsoft%20365%20Defender-green?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Role-SOC%20Analyst-orange?style=for-the-badge"/>
</p>
