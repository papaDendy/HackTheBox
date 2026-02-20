# Redeemer

> Platform: Hack The Box  
> Difficulty: Very Easy  
> Category: Starting Point  

---

## 🎯 Objective

Identify exposed Redis service and retrieve the flag through unauthenticated access.

---

## 🔎 Attack Surface

- Open ports: 6379/tcp  
- Service: Redis  
- Key finding: No authentication required  

---

## ⚙️ Exploitation Overview

1. Full TCP scan identified Redis service.
2. Connected via netcat.
3. Enumerated available keys.
4. Retrieved flag value.

---

## 🧠 Root Cause

Redis service exposed externally without authentication.

---

## 🛡 Mitigation

- Bind Redis to localhost  
- Enable authentication (`requirepass`)  
- Restrict access via firewall  

---

## ⚠ Disclaimer

This write-up is for educational purposes only.
