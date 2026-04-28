# B27 – Intrusion Detection System Testing

This section demonstrates the application of a cybersecurity concept by testing an intrusion detection system (IDS) in a controlled environment. The experiment evaluates how effectively the IDS detects simulated attack behaviour.

---

## Intrusion Detection System Testing (Snort)

### Description  
An intrusion detection system (IDS) monitors network traffic to identify suspicious or malicious activity. In this experiment, a network-based IDS was tested against common attack techniques such as port scanning and brute-force login attempts.

---

### Evidence  
<img width="858" height="705" alt="image" src="https://github.com/user-attachments/assets/b58848be-ea1e-4dc8-a99a-9c00248c1151" />
<img width="864" height="709" alt="image" src="https://github.com/user-attachments/assets/c9b099ca-ae88-4458-bbc0-e4485e265a1c" />
<img width="864" height="709" alt="image" src="https://github.com/user-attachments/assets/dffe0e45-cc8a-4af3-87f6-c82f6c79e7cd" />





---

### Explanation  
The IDS used in this experiment was Snort, configured on a Kali Linux environment. It was executed using:

```bash
sudo snort -c /etc/snort/snort.lua -i eth0
