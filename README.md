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


---

## 👤 Author
**Jaden Julius Mascarenhas**  
Cybersecurity Analyst — SOC / IR / GRC  
Master’s in Information & Network Security (Kingston University)

---

## 📄 License
Educational & professional development use.

