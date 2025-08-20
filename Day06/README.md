# OWASP Top 10 – Web Application Security

The **OWASP Top 10** is a standard awareness document for developers and security professionals.  
It represents the most critical web application security risks.

---

## 1. Broken Access Control
Users can act outside their intended permissions.  

**Example:** Accessing another user’s account or admin panel.

---

## 2. Cryptographic Failures
Sensitive data exposure due to weak or no encryption.  

**Example:** Transmitting credentials in plain text → vulnerable to *Man-in-the-Middle Attack*.

---

## 3. Injection
Untrusted data is sent to an interpreter (SQL, OS, LDAP, etc.).  

**Example:** SQL Injection / Command Injection
```sql
SELECT * FROM users WHERE username = 'admin' --' AND password = '';
````

---

## 4. Insecure Design

Weak security controls in the system design phase.

**Examples:**

* CAPTCHA can be bypassed
* File upload allows `.exe` but blocks `.png`

---

## 5. Security Misconfiguration

Default configurations, incomplete setups, open cloud storage, or unnecessary features enabled.

**Example:** Leaving admin console publicly accessible.

---

## 6. Vulnerable and Outdated Components

Using outdated frameworks, libraries, or modules.

**Example:** Apache server vulnerabilities.

---

## 7. Identification and Authentication Failures

Weak or broken authentication mechanisms.

**Example:** Session ID exposed or weak password enforcement.

---

## 8. Software and Data Integrity Failures

Untrusted software updates, insecure CI/CD pipelines, or reliance on unverified plugins.

**Example:** Malicious code injected during a software update.

---

## 9. Security Logging and Monitoring Failures

Attacks not detected due to insufficient logging.

**Example:** No alerting for repeated failed login attempts.

---

## 10. Server-Side Request Forgery (SSRF)

Attacker tricks the server into making requests to unintended locations.

**Example:** Accessing internal resources via manipulated URL input.

---
