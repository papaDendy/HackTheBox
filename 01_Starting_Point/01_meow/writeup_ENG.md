# Meow — Write-Up

## Summary

The machine is vulnerable due to an exposed Telnet service that allows root access without requiring a password.

---

## Recon

A full TCP port scan revealed that port 23 (Telnet) was open.

---

## Enumeration

The Telnet service did not require authentication.

Logging in as the root user was possible without providing a password.

---

## Exploitation

After successful login, full access to the file system was obtained.

The flag was located in the root directory and successfully retrieved.

---

## Root Cause

- Telnet service exposed to external networks
- Root account configured without a password
- Use of an insecure remote access protocol

---

## Mitigation

- Disable Telnet service
- Replace Telnet with SSH
- Disable direct root login
- Enforce strong authentication policies