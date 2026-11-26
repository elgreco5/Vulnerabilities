# **Security Advisory**

## **Summary**

Stored Cross-Site Scripting (XSS)

---

## **Description**

OpenMetadata up to version 1.12.14 is vulnerable to **Stored Cross-Site Scripting (XSS)** in the description field of created objects.
The application fails to properly neutralize user-supplied input that uses alternative or obfuscated JavaScript syntax, allowing malicious scripts to be executed in the victim’s browser.

---

## **Impact**

A Cross-Site Scripting (XSS) vulnerability via the description field allows attackers to execute arbitrary JavaScript and access sensitive browser storage, such as JSON Web Tokens (JWT), leading to session hijacking or privilege escalation.

---

## **Affected Versions**

<=1.12.14

---


## **Patched Versions**

1.13.0 and above

---


## **CWE**

CWE-79

---

## **CVSS**

**8.0 – High**
`CVSS:3.1/AV:N/AC:L/PR:L/UI:R/S:U/C:H/I:H/A:H`

---

## **References**

CWE-79 - Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')
