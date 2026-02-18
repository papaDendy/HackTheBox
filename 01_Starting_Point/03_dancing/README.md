# Dancing

> Platform: Hack The Box  
> Difficulty: Very Easy  
> Category: Starting Point  

---

## 🎯 Objective

Enumerate SMB service and retrieve the flag from an accessible network share.

---

## 🔎 Attack Surface

- Open ports: 135/tcp, 139/tcp, 445/tcp  
- Service: SMB  
- Key finding: Accessible share without strict access controls  

---

## ⚙️ Exploitation Overview

1. Full TCP scan identified SMB service.
2. Enumerated available shares.
3. Accessed readable share.
4. Retrieved flag file.

---

## 🧠 Root Cause

Improperly configured SMB share with insufficient access restrictions.

---

## 🛡 Mitigation

- Restrict SMB exposure
- Disable anonymous access
- Apply strict ACL policies

---

## ⚠ Disclaimer

This write-up is for educational purposes only.
