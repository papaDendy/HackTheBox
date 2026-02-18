# Dancing — Lab Notes

## Target
IP: <TARGET_IP>

---

# Recon

nmap -p- -sS -T4 --min-rate 1000 <TARGET_IP>

Result:
135/tcp open msrpc
139/tcp open netbios-ssn
445/tcp open microsoft-ds

---

# Service Scan

nmap -sV -p 135,139,445 <TARGET_IP>

SMB service detected.

---

# Enumeration

smbclient -L //<TARGET_IP>/

Shares discovered.

smbclient //<TARGET_IP>/<SHARE_NAME>

Connected successfully.

ls
get flag.txt

Flag retrieved.
