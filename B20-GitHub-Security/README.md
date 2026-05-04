# B20 – Enhancing GitHub Project Security

This section demonstrates how the security of a GitHub repository was improved using built-in security features. The implementation focuses on detecting vulnerabilities, preventing sensitive data exposure, and strengthening overall code security.

---

## Description

The security of the repository was enhanced by enabling key GitHub security tools. These tools provide automated protection against common risks such as vulnerable dependencies, insecure code, and leaked credentials.

---

## Implemented Security Measures

### 1. Dependabot Alerts & Security Updates
Dependabot was enabled to automatically detect vulnerable dependencies and provide security updates. This ensures that outdated or insecure libraries are identified and patched promptly.

### 2. CodeQL Code Scanning
CodeQL was configured and successfully executed to analyze the repository’s code. A sample Python file was added to enable scanning, allowing GitHub to detect potential vulnerabilities and unsafe coding practices.

### 3. Secret Scanning
Secret scanning was enabled to detect exposed sensitive information such as API keys, tokens, or passwords. This helps prevent accidental data leaks and unauthorized access.

---

## Why This Improves Security

These features improve security by providing automated and continuous monitoring of the repository. Dependabot secures dependencies, CodeQL strengthens code quality through static analysis, and secret scanning prevents credential exposure. Together, they form a strong foundation for secure software development.

---

## Evidence
<img width="1600" height="722" alt="image" src="https://github.com/user-attachments/assets/11b35f4e-b9bd-4025-ae99-0bf076b44d26" />
<img width="1218" height="757" alt="image" src="https://github.com/user-attachments/assets/8c79f60c-873b-457d-a9ac-414cca1493f7" />
<img width="1919" height="903" alt="image" src="https://github.com/user-attachments/assets/e7049854-9fe1-4aaa-8c56-0aeab9a0b645" />


---

## Reflection

This task demonstrated how simple configurations can significantly improve repository security. It highlights the importance of proactive security measures in real-world development, where automated tools play a key role in identifying and mitigating risks early.
