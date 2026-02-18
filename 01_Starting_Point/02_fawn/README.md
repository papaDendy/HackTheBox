# Fawn

> Platform: Hack The Box  
> Difficulty: Very Easy  
> Category: Starting Point  

---

## 🎯 Objective

Identify exposed FTP service and retrieve the flag using anonymous access.

---

## 🔎 Attack Surface

- Open ports: 21/tcp  
- Service: FTP  
- Key finding: Anonymous login enabled  

---

## ⚙️ Exploitation Overview

1. Full TCP scan identified FTP service.
2. Connected using anonymous credentials.
3. Listed available files.
4. Retrieved flag file.

---

## 🧠 Root Cause

Misconfigured FTP server allowing anonymous access to sensitive files.

---

## 🛡 Mitigation

- Disable anonymous FTP access  
- Restrict external exposure  
- Implement proper authentication controls  

---

## ⚠ Disclaimer

This write-up is for educational purposes only.
