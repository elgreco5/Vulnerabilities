# **Security Advisory**

## **Summary**

Stored Cross-Site Scripting (XSS)

---

## **Description**

OpenMetadata up to version 1.12.14 is vulnerable to **Stored Cross-Site Scripting (XSS)** in the description field of created objects.
The application fails to properly neutralize user-supplied input that uses alternative or obfuscated JavaScript syntax, allowing malicious scripts to be executed in the victim’s browser.

---

## **Impact**

An attacker may exploit this vulnerability to execute arbitrary JavaScript, steal session tokens, hijack user sessions, manipulate application content, and facilitate phishing or privilege escalation attacks.

---

## **Affected Versions**

* OpenMetadata up to version 1.12.14

---

## **CWE**

* CWE-79

---

## **CVSS**

**8.0 – High**
`CVSS:3.1/AV:N/AC:L/PR:L/UI:R/S:U/C:H/I:H/A:H`

---

## **References**

* CWE-79 - Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')
