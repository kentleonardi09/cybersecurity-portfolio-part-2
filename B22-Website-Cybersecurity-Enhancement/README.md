# B22 – Website Cybersecurity Enhancement

## Website Analysed  
https://saintmarys.au/

---

## Purpose  
To identify cybersecurity risks in a community website and propose practical improvements to enhance security and reduce vulnerabilities.

---

## Tools Used  
- Kali Linux  
- OWASP ZAP  

---

## Key Improvements  

### 1. Security Headers  
Missing headers such as CSP, HSTS, and X-Frame-Options increase risk of XSS and clickjacking.  
**Fix:** Add proper security headers  

---

### 2. Secure Cookies  
Cookies lack HttpOnly, Secure, and SameSite attributes, increasing risk of session hijacking.  
**Fix:** Configure secure cookie settings  

---

### 3. Anti-CSRF Protection  
No CSRF tokens detected, allowing potential unauthorized actions.  
**Fix:** Implement and validate CSRF tokens  

---

### 4. Content Security Policy (CSP)  
Weak or missing CSP (unsafe-inline, wildcard) allows malicious scripts.  
**Fix:** Restrict sources and remove unsafe rules  

---

## Evidence (OWASP ZAP Findings)

- Absence of Anti-CSRF Tokens  
- Content Security Policy (CSP) Header Not Set  
- CSP Wildcard Directive  
- CSP script-src unsafe-inline  
- CSP style-src unsafe-inline  
- Missing Anti-clickjacking Header  
- Cookie No HttpOnly Flag  
- Cookie Without Secure Flag  
- Cookie without SameSite Attribute  

---

## Conclusion  
Applying these improvements strengthens the website’s security and reduces common web vulnerabilities.
