# B2 – Discover 5 Unique Strong Security Implementations

This section presents five distinct strong security implementations, supported by real-world evidence, examples, and analysis.

---

## 1. Input Validation and Parameterized Queries

### Description
A strong security implementation ensures that user input is handled securely using techniques such as parameterized queries to prevent injection attacks.

### Evidence
<img width="1303" height="680" alt="WhatsApp Image 2026-04-15 at 10 53 48 PM" src="https://github.com/user-attachments/assets/82900e66-0ca9-4ee5-a51a-74a7c1f42897" />


### Explanation
As shown in the evidence, the application uses prepared statements with placeholders (`?`) instead of directly inserting user input into SQL queries. This ensures that user input is treated strictly as data rather than executable code. Even when malicious input is provided, the structure of the query remains unchanged, effectively preventing SQL Injection attacks.

---

## 2. Secure Credential Storage (Hashing and Salting)

### Description
A strong security implementation ensures that user credentials are securely stored using hashing algorithms combined with salting techniques.

### Evidence
<img width="1208" height="667" alt="WhatsApp Image 2026-04-15 at 10 57 22 PM" src="https://github.com/user-attachments/assets/48c92bc8-226b-4f3c-94a8-9620b2cdf448" />
<img width="1130" height="472" alt="WhatsApp Image 2026-04-15 at 10 58 34 PM" src="https://github.com/user-attachments/assets/7d3f40c8-58f9-44d5-a951-bf5a91f078ef" />


### Explanation
As shown in the evidence, bcrypt is used to hash passwords securely while incorporating a salt by default. The implementation demonstrates how increasing the cost factor makes the hashing process more computationally intensive. This significantly reduces the effectiveness of brute-force and dictionary attacks, ensuring that even if credentials are exposed, they cannot be easily reversed.

---

## 3. Role-Based Access Control (Least Privilege)

### Description
A strong security implementation enforces access control by ensuring that users are granted only the minimum level of access required to perform their tasks.

### Evidence
<img width="750" height="268" alt="WhatsApp Image 2026-04-15 at 11 01 39 PM" src="https://github.com/user-attachments/assets/fbc5c985-e3f2-4614-b637-b059262755cf" />


### Explanation
As shown in the evidence, the system implements the principle of least privilege by distinguishing between administrative and standard user roles. Access to sensitive operations is restricted, and additional controls such as auditing and monitoring are applied. This ensures that users cannot access or modify resources beyond their authorized permissions, reducing the risk of unauthorized access.

---

## 4. Input Sanitization and Output Encoding (XSS Prevention)

### Description
A strong security implementation ensures that all user input is properly sanitized before being rendered in a web application.

### Evidence
<img width="883" height="684" alt="WhatsApp Image 2026-04-15 at 11 05 50 PM" src="https://github.com/user-attachments/assets/0cf7d4d1-88ea-436c-a6d5-5d1f61655af6" />


### Explanation
As shown in the evidence, HTML sanitization is performed using DOMPurify to remove potentially dangerous content from user input. This ensures that malicious scripts are stripped before rendering, preventing execution in the browser and effectively mitigating Cross-Site Scripting (XSS) attacks.

---

## 5. Multi-Factor Authentication (MFA)

### Description
A strong security implementation enhances authentication by requiring multiple forms of verification from the user.

### Evidence
<img width="208" height="465" alt="WhatsApp Image 2026-04-15 at 11 09 57 PM" src="https://github.com/user-attachments/assets/30466a98-e1c1-440f-80f9-ec74cfc2bcba" />


### Explanation
As shown in the evidence, an authenticator application generates time-based one-time passwords (OTP) that are required in addition to the user’s password. These codes change frequently and provide an additional layer of security. This ensures that even if a password is compromised, unauthorized access is prevented.

---

## Final Reflection

These strong security implementations demonstrate the importance of incorporating security best practices into system design. By applying techniques such as input validation, secure credential storage, access control, sanitization, and multi-factor authentication, systems can effectively mitigate common vulnerabilities and improve overall security resilience.
