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
<img width="868" height="703" alt="WhatsApp Image 2026-04-29 at 2 55 25 PM" src="https://github.com/user-attachments/assets/dadced56-0209-4f8e-8ffa-617d74de067d" />
<img width="1255" height="1015" alt="WhatsApp Image 2026-04-29 at 3 01 50 PM" src="https://github.com/user-attachments/assets/6cc11f89-5059-49ff-b430-706a827b475e" />


---

## Conclusion  
Applying these improvements strengthens the website’s security and reduces common web vulnerabilities.
