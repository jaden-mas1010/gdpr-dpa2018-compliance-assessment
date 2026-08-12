## 🧭 Executive Summary

This assessment reviews a simulated web application’s alignment with the **General Data Protection Regulation (GDPR)** and the **UK Data Protection Act 2018 (DPA 2018)**. The application processes basic personal data, including names, email addresses, and login credentials. Several technical weaknesses were identified that directly impact the confidentiality, integrity, and lawful processing of personal data.

The most critical issues include:
- **Unencrypted transport (HTTP)** exposing user credentials and personal data.
- **Missing security headers**, increasing exposure to common web attacks.
- **Excessive logging of personal data**, violating data minimisation principles.
- **Weak password policy**, increasing the likelihood of account compromise.

These findings map to GDPR Articles **5**, **25**, **30**, **32**, and **33**, indicating gaps in secure processing, privacy‑by‑design, and breach readiness. Addressing these issues strengthens both the technical security posture and regulatory compliance of the application.

This executive summary provides leadership and auditors with a high‑level understanding of risks, impacts, and required remediation actions.
