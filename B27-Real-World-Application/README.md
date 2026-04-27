# B27 - Apply a Learned Concept to a Real-World Application

This section demonstrates the application of a cybersecurity concept learned in this unit to a real-world scenario, focusing on password security and hashing techniques.

---

## 1. Password Hashing (SHA-256)

### Description
I used SHA-256 to hash a password and observed that the same password always produces the same hash when no salt is applied. This shows that unsalted hashing is deterministic.

```bash
echo -n "password123" | sha256sum

### Evidence
<img width="949" height="316" alt="image" src="https://github.com/user-attachments/assets/8d190779-483e-4b8e-a78b-5fcde786c80c" />
<img width="916" height="912" alt="image" src="https://github.com/user-attachments/assets/dfb3d3fb-0119-4d46-bdf4-b021994d8aba" />
<img width="583" height="56" alt="image" src="https://github.com/user-attachments/assets/cb12d657-4850-4d09-95bf-270e98f5180d" />


