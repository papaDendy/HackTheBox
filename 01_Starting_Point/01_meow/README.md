# Meow

> Platform: Hack The Box  
> Difficulty: Very Easy  
> Category: Starting Point  

---

## 🎯 Objective

Identify and exploit exposed Telnet service to retrieve the flag.

---

## 🔎 Attack Surface

- Open ports: 23/tcp  
- Service: Telnet  
- Key finding: root login without password  

---

## ⚙️ Exploitation Overview

1. Full TCP scan identified open Telnet service.
2. Connected via Telnet.
3. Logged in as root without authentication.
4. Retrieved flag from root directory.

---

## 🧠 Root Cause

Insecure service exposed to the internet with no authentication controls.

---

## 🛡 Mitigation

- Disable Telnet
- Enforce authentication
- Replace with SSH

---

## ⚠ Disclaimer

This write-up is for educational purposes only.
