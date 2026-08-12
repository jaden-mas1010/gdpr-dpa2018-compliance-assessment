# GDPR & UK DPA 2018 Compliance Assessment
*A security‑driven compliance review of a simulated web application, mapping technical findings to regulatory obligations and providing SOC‑style remediation.*

---

## 📌 Overview
This project evaluates a simulated web application against **GDPR** and the **UK Data Protection Act 2018**, demonstrating how technical vulnerabilities translate into **legal risk**, **business impact**, and **actionable remediation**.

It showcases the ability to bridge **technical security testing**, **SOC‑style analysis**, and **governance/compliance requirements** — a key skillset for modern cybersecurity roles.

---

## 🎯 Objectives
- Identify security weaknesses affecting personal data processing  
- Map each finding to GDPR/DPA 2018 articles  
- Assess risk severity using SOC‑aligned methodology  
- Provide clear, prioritized remediation steps  
- Demonstrate technical → legal translation skills  

---

## 🔍 Methodology

### Technical Testing
- **Nmap** — TLS & service enumeration  
- **Nikto** — web server misconfiguration scanning  
- **Burp Suite** — manual HTTP inspection  
- **Suricata IDS** — log review & PII exposure checks  

### Compliance Mapping
- GDPR Articles **5**, **25**, **30**, **32**, **33**  
- UK DPA 2018 principles  
- CIA‑based impact scoring  
- Likelihood × impact risk classification  

### Reporting
- SOC‑style remediation  
- Business impact explanation  
- Evidence‑based findings  

---

## 🛡 Key Findings & GDPR/DPA Mapping

### 1. Insecure Transport (HTTP instead of HTTPS)
**Risk:** Cleartext transmission of credentials & personal data  
**GDPR/DPA Impact:**  
- Art. 5(1)(f) — Integrity & confidentiality  
- Art. 32 — Appropriate security controls  
- Art. 33 — Breach notification if exploited  
**Remediation:** Enforce TLS 1.2+, enable HSTS, secure cookies, disable weak ciphers  

---

### 2. Missing Security Headers
**Risk:** Exposure to clickjacking, XSS, MIME‑type confusion  
**GDPR/DPA Impact:**  
- Art. 25 — Privacy‑by‑design  
- Art. 32 — Insufficient hardening  
**Remediation:** Implement CSP, X‑Frame‑Options, X‑Content‑Type‑Options, Referrer‑Policy  

---

### 3. Excessive Logging of Personal Data
**Risk:** Logs contain unnecessary PII, increasing breach impact  
**GDPR/DPA Impact:**  
- Art. 5(1)(c) — Data minimisation  
- Art. 30 — Records of processing  
**Remediation:** Redact PII, apply log rotation, enforce retention limits, restrict access  

---

### 4. Weak Password Policy
**Risk:** Higher likelihood of account compromise  
**GDPR/DPA Impact:**  
- Art. 32 — Inadequate protection  
**Remediation:** Enforce strong complexity, rate limiting, MFA, secure hashing  

---

## 🛠 Tools Used
- Nmap  
- Nikto  
- Burp Suite  
- Suricata IDS  
- Manual log analysis  

---

## 📈 Outcome
This assessment demonstrates how technical testing supports GDPR & UK DPA 2018 compliance by addressing:

- Secure processing  
- Data minimisation  
- Privacy‑by‑design  
- Breach readiness  
- Logging & retention hygiene  
- Authentication hardening  

It serves as a practical, portfolio‑ready example for:

- SOC analysts  
- Security engineers  
- GRC practitioners  
- Academic coursework  

---
## 🧭 Executive Summary

This assessment reviews a simulated web application’s alignment with the **General Data Protection Regulation (GDPR)** and the **UK Data Protection Act 2018 (DPA 2018)**. The application processes basic personal data, including names, email addresses, and login credentials. Several technical weaknesses were identified that directly impact the confidentiality, integrity, and lawful processing of personal data.

The most critical issues include:
- **Unencrypted transport (HTTP)** exposing user credentials and personal data.
- **Missing security headers**, increasing exposure to common web attacks.
- **Excessive logging of personal data**, violating data minimisation principles.
- **Weak password policy**, increasing the likelihood of account compromise.

These findings map to GDPR Articles **5**, **25**, **30**, **32**, and **33**, indicating gaps in secure processing, privacy‑by‑design, and breach readiness. Addressing these issues strengthens both the technical security posture and regulatory compliance of the application.

This executive summary provides leadership and auditors with a high‑level understanding of risks, impacts, and required remediation actions.

## ⚠️ Risk Matrix

The following matrix evaluates each identified issue based on **Likelihood** and **Impact**, using a standard SOC/GRC scoring model. This helps prioritise remediation and communicate risk clearly to stakeholders.

| Risk Level | Likelihood | Impact | Description |
|-----------|------------|--------|-------------|
| **Critical** | High | High | Direct exposure of personal data or credentials; immediate regulatory and security risk. |
| **High** | Medium–High | High | Significant vulnerability affecting confidentiality, integrity, or lawful processing of personal data. |
| **Medium** | Medium | Medium | Weaknesses that increase attack surface or violate GDPR principles but require chaining to exploit. |
| **Low** | Low | Low–Medium | Minor misconfigurations with limited security or compliance impact. |

### **Mapped Risks for This Assessment**

| Issue | Likelihood | Impact | Risk Level | Notes |
|-------|------------|--------|------------|-------|
| **Unencrypted HTTP transport** | High | High | **Critical** | Credentials & PII exposed in cleartext; violates Art. 5(1)(f) & Art. 32. |
| **Missing security headers** | Medium | High | **High** | Increased exposure to XSS, clickjacking; violates Art. 25 & Art. 32. |
| **Excessive logging of PII** | Medium | Medium–High | **High** | Violates data minimisation (Art. 5(1)(c)); increases breach impact. |
| **Weak password policy** | Medium | Medium | **Medium** | Higher likelihood of account compromise; violates Art. 32. |

This matrix provides a clear, defensible prioritisation for remediation and aligns with SOC and GRC reporting standards.

---

## 👤 Author
**Jaden Julius Mascarenhas**  
Cybersecurity Analyst — SOC / IR / GRC  
Master’s in Information & Network Security (Kingston University)

---

## 📄 License
Educational & professional development use.

