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

nmap -sV -p  <TARGET_IP>

Service:
Apache httpd 2.4.38 ((Debian))



---

# Exploitation

