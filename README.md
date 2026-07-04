GDPR & UK DPA 2018 Compliance Assessment
1. Introduction
This project presents a practical GDPR and UK Data Protection Act 2018 compliance assessment performed on a simulated web application. The goal is to demonstrate how technical security findings discovered through common security tools can be translated into legal and regulatory obligations — a core skill for SOC analysts, security engineers, and compliance‑driven cybersecurity roles in the UK.

The assessment focuses on identifying weaknesses in transport security, logging practices, security headers, and authentication controls, and then mapping each issue to relevant GDPR Articles and DPA 2018 principles. This bridges the gap between hands‑on technical testing and real‑world compliance expectations.

2. Project Scope
Target
A dummy/simulated web application designed to mimic a typical small‑scale service handling basic personal data.

Data Processed
Name

Email address

Login credentials (username/password)

Assessment Focus
Transport layer security

Application security headers

Logging and data minimisation

Password and authentication policies

Breach readiness and secure processing obligations

3. Methodology
The assessment follows a simple, repeatable workflow:

Reconnaissance & Scanning

Nmap for service discovery and TLS checks

Nikto for web server misconfigurations

Application Testing

Burp Suite for manual inspection of HTTP traffic

Header analysis (CSP, HSTS, X‑Frame‑Options, etc.)

Log Review

Suricata IDS logs

Manual inspection of application logs for PII exposure

Compliance Mapping

Each technical finding is mapped to GDPR Articles 5, 25, 30, 32, and 33

Relevant UK DPA 2018 principles are referenced where applicable

Recommendations

SOC‑style remediation steps

Practical hardening measures

4. Key Findings & GDPR/DPA‑2018 Mapping
4.1 Insecure Transport (HTTP instead of HTTPS)
Technical Risk:  
Credentials and personal data transmitted in cleartext, vulnerable to interception.

GDPR/DPA Impact:

Article 5(1)(f): Integrity & confidentiality

Article 32: Failure to implement appropriate security controls

Article 33: Breach notification required if exploited

Recommendation:  
Enforce TLS 1.2+, enable HSTS, secure cookies, and disable weak ciphers.

4.2 Missing Security Headers
Technical Risk:  
Exposure to clickjacking, XSS, MIME‑type confusion, and other client‑side attacks.

GDPR/DPA Impact:

Article 25: Lack of privacy‑by‑design controls

Article 32: Insufficient hardening measures

Recommendation:  
Implement CSP, X‑Frame‑Options, X‑Content‑Type‑Options, Referrer‑Policy.

4.3 Excessive Logging of Personal Data
Technical Risk:  
Logs contain unnecessary PII, increasing breach impact and retention liability.

GDPR/DPA Impact:

Article 5(1)(c): Data minimisation

Article 30: Records of processing activities

Recommendation:  
Redact PII, apply log rotation, enforce retention limits, and restrict access.

4.4 Weak Password Policy
Technical Risk:  
Higher likelihood of account compromise and unauthorised access.

GDPR/DPA Impact:

Article 32: Inadequate protection of personal data

Recommendation:  
Enforce strong password complexity, rate limiting, MFA, and secure hashing.

5. Tools Used
Nmap — service discovery, TLS checks

Nikto — web server vulnerability scanning

Burp Suite — manual HTTP inspection

Suricata IDS — network traffic and alert review

Manual log analysis — PII exposure and retention issues

6. Outcome
This project demonstrates how technical security assessments directly support GDPR and UK DPA 2018 compliance. By mapping vulnerabilities to legal obligations, the assessment highlights the importance of:

Secure processing

Data minimisation

Privacy‑by‑design

Breach readiness

Proper logging and retention

Strong authentication controls

The result is a concise, practical example of compliance‑aware security testing suitable for academic submissions, SOC analyst portfolios, and professional development.

7. Repository Structure
Code
GDPR-DPA2018-Compliance-Assessment/
│
├── README.md
├── report.md
├── mapping-table.md
├── recommendations.md
│
└── findings/
    ├── nmap-scan.png
    ├── nikto-output.txt
    ├── burp-http-traffic.png
    └── suricata-alerts.json
8. License
This project is provided for educational and professional development purposes.
