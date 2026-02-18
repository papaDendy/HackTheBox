# Fawn — Write-Up

## Summary

The machine is vulnerable due to an exposed FTP service that allows anonymous login.

---

## Recon

A full TCP scan revealed port 21 (FTP) open.

---

## Enumeration

The FTP service allowed anonymous authentication.

After logging in as `anonymous`, directory listing was permitted.

---

## Exploitation

Using the FTP client, the flag file was identified and downloaded.

The flag was successfully retrieved.

---

## Root Cause

- FTP service exposed externally
- Anonymous login enabled
- Lack of access control

---

## Mitigation

- Disable anonymous access
- Restrict FTP exposure via firewall
- Enforce authentication policies
