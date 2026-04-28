# B24 – Access Control Implementation

This section demonstrates the design and implementation of an access control mechanism using built-in Linux file permissions.

---

## Description  
Access control ensures that only authorized users can access specific resources. In this experiment, access control was implemented using Linux file permission settings in a Kali Linux environment.

---

## Evidence  
<img width="857" height="712" alt="image" src="https://github.com/user-attachments/assets/d3cbd540-57a3-48b4-8cc7-d2d92abb05a4" />


---

## Explanation  
A file containing sensitive data was created and its permissions were modified using the `chmod` command. Initially, all permissions were removed, preventing access to the file. Permissions were then updated to allow only the file owner to read and write.

Commands used:

```bash
echo "Sensitive Data" > secret.txt
chmod 000 secret.txt
cat secret.txt
chmod 600 secret.txt
cat secret.txt
ls -l secret.txt
