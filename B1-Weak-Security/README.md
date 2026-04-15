# B1 – Discover 5 Unique Weak/Vulnerable Security Implementations

This section presents five distinct weak security implementations, supported by real-world evidence, examples, and analysis.

---

## 1. Weak Input Validation (SQL Injection – CWE-89)

### Description
A weak security implementation occurs when user input is not properly validated or sanitized before being processed by the system.

### Evidence
<img width="1600" height="722" alt="WhatsApp Image 2026-04-15 at 9 53 24 PM" src="https://github.com/user-attachments/assets/8a6ade5b-5f8a-42a9-ad74-05de7ca2c223" />


### Explanation
As shown in the evidence, user-controlled input is directly incorporated into an SQL query without proper validation. This allows attackers to inject malicious input, such as `' OR '1'='1`, which alters the logic of the query and bypasses authentication mechanisms. As a result, unauthorized access to the database can be achieved, demonstrating a critical security flaw.

---

## 2. Hardcoded Credentials (CWE-798)

### Description
A weak security implementation occurs when sensitive credentials are embedded directly within the source code instead of being securely stored.

### Evidence
<img width="1600" height="559" alt="image" src="https://github.com/user-attachments/assets/b78eba32-cb9a-4090-b9e6-1f74aa860e3d" />


### Explanation
As demonstrated in the evidence, the password is hardcoded within the application code, making it visible to anyone with access to the source. This significantly weakens the authentication process, as attackers can easily extract and use the credentials to gain unauthorized access without needing to exploit additional vulnerabilities.

---

## 3. Improper Access Control (CWE-284)

### Description
A weak security implementation occurs when a system fails to enforce appropriate access restrictions, allowing users to access resources beyond their authorized permissions.

### Evidence
<img width="1600" height="401" alt="image" src="https://github.com/user-attachments/assets/ea4f5ae2-4a3a-40df-8201-316c388d2cc8" />


### Explanation
As shown in the evidence, the system processes requests and retrieves data without verifying whether the user is authorized to access the requested information. This lack of authorization checks enables unauthorized users to access sensitive data, demonstrating a failure to enforce proper access control mechanisms.

---

## 4. Improper Input Sanitization (Cross-Site Scripting – CWE-79)

### Description
A weak security implementation occurs when user input is not properly sanitized or encoded before being displayed in a web application.

### Evidence
<img width="1600" height="540" alt="image" src="https://github.com/user-attachments/assets/bea7f74a-3ad9-4b5c-8d09-5c37401b129d" />


### Explanation
As illustrated in the evidence, malicious scripts can be injected into the application through user input and subsequently executed in other users’ browsers. This demonstrates that the system fails to sanitize input effectively, allowing attackers to execute arbitrary scripts, potentially leading to data theft or session hijacking.

---

## 5. Weak Authentication Mechanisms (Weak Password Policy – CWE-521)

### Description
A weak security implementation occurs when systems allow users to create simple and easily guessable passwords.

### Evidence
<img width="1600" height="489" alt="image" src="https://github.com/user-attachments/assets/703a2ab3-10c8-4c5e-a4e4-0869a592aeb7" />


### Explanation
As shown in the evidence, weak passwords that are short, predictable, or based on common patterns can be easily compromised through brute-force or dictionary attacks. This significantly reduces the effectiveness of authentication mechanisms and increases the likelihood of unauthorized access.

---

## Final Reflection

These examples demonstrate that weak security implementations often arise from inadequate design decisions and poor coding practices, such as insufficient input validation, improper access control, and weak authentication mechanisms. Such weaknesses can lead to serious consequences, including unauthorized access, data breaches, and system compromise. Addressing these issues requires the adoption of secure coding practices and the implementation of robust security controls throughout the system development lifecycle.
