# Executive Summary

This assessment reviews a simulated web application’s alignment with the General Data Protection Regulation (GDPR) and the UK Data Protection Act 2018 (DPA 2018). The application processes basic personal data, including names, email addresses, and login credentials.

Several critical weaknesses were identified:

- Unencrypted HTTP transport exposing credentials and personal data.
- Missing security headers increasing exposure to client-side attacks.
- Excessive logging of personal data, violating data minimisation principles.
- Weak password policy increasing likelihood of account compromise.

These findings map to GDPR Articles 5, 25, 30, 32, and 33, indicating gaps in secure processing, privacy-by-design, and breach readiness.

This summary provides leadership with a high-level understanding of risks, impacts, and required remediation actions.
