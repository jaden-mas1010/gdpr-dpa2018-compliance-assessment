# Technical Findings

## 1. Insecure Transport (HTTP)
**Description:** Application uses HTTP instead of HTTPS.  
**Evidence:** Nmap scan shows port 80 open with no TLS.  
**Impact:** Credentials and PII transmitted in cleartext.  
**GDPR/DPA Mapping:** Art. 5(1)(f), Art. 32.  
**Severity:** Critical.

## 2. Missing Security Headers
**Description:** No CSP, HSTS, X-Frame-Options, or Referrer-Policy.  
**Evidence:** Burp Suite header inspection.  
**Impact:** Exposure to clickjacking, XSS, MIME-type confusion.  
**GDPR/DPA Mapping:** Art. 25, Art. 32.  
**Severity:** High.

## 3. Excessive Logging of PII
**Description:** Suricata logs contain unnecessary personal data.  
**Impact:** Increased breach impact; violates data minimisation.  
**GDPR/DPA Mapping:** Art. 5(1)(c), Art. 30.  
**Severity:** High.

## 4. Weak Password Policy
**Description:** No complexity requirements or rate limiting.  
**Impact:** Higher likelihood of account compromise.  
**GDPR/DPA Mapping:** Art. 32.  
**Severity:** Medium.
