# Appointment

> Platform: Hack The Box  
> Difficulty: Very Easy  
> Category: Starting Point (Web)  

---

## 🎯 Objective

Identify and exploit a SQL Injection vulnerability in a web login form to retrieve the flag.

---

## 🔎 Attack Surface

- Open ports: 80/tcp  
- Service: HTTP  
- Key finding: Login form vulnerable to SQL Injection  

---

## ⚙️ Exploitation Overview

1. Web service discovered on port 80.
2. Login form identified.
3. SQL Injection payload used to bypass authentication.
4. Access granted and flag retrieved.

---

## 🧠 Root Cause

Improper handling of user input in SQL query construction.

---

## 🛡 Mitigation

- Use parameterized queries (Prepared Statements)
- Implement server-side input validation
- Deploy Web Application Firewall (WAF)

---

## ⚠ Disclaimer

This write-up is for educational purposes only.
