# Networkwalks-B082-week4-Medirozahospital-Security-project
# 🔐 Mediroza Hospital – Security Assessment

### **Authorized Cybersecurity / Penetration Testing Project**

A controlled security assessment of the **Mediroza Hospital web application**, conducted as part of the **NETWORKWALKS Cybersecurity Internship – Batch B082**.

This project focuses on identifying security weaknesses related to authentication, access control, sensitive data exposure, database security, and password/hash protection.

> ⚠️ **Educational & Authorized Assessment Only**

---

## 📌 Project Overview

This repository documents a structured security assessment performed against the Mediroza Hospital application in an authorized and controlled environment.

The assessment was divided into multiple milestones to identify potential vulnerabilities and evaluate their security impact.

The project covers:

* Initial access and authentication testing
* Web application security assessment
* Sensitive data exposure
* Database security assessment
* Password and hash security
* Risk analysis
* Security recommendations
* Evidence collection and documentation

All activities were performed within an authorized cybersecurity lab environment.

---

## 🎯 Objectives

The main objectives of this assessment were:

*  Identify authentication weaknesses
*  Evaluate access-control mechanisms
*  Assess sensitive information exposure
*  Analyze database security
*  Evaluate password and hash protection
*  Perform controlled security testing
*  Collect evidence of findings
*  Classify vulnerabilities according to risk
*  Provide practical remediation recommendations
*  Prepare professional security documentation

---

## 🧪 Assessment Methodology

The assessment followed a structured penetration-testing workflow:

```text
Reconnaissance
      ↓
Application Analysis
      ↓
Authentication Assessment
      ↓
Access-Control Testing
      ↓
Data Exposure Assessment
      ↓
Database Security Assessment
      ↓
Password / Hash Assessment
      ↓
Risk Analysis
      ↓
Remediation
      ↓
Final Report
```

---

# 📂 Assessment Milestones

## 🔹 M1 – Initial Access

### Focus

* Application analysis
* Login functionality
* Authentication workflow
* HTTP request/response inspection
* Access-control validation
* Controlled input testing
* Evidence collection

### Objective

Determine whether weaknesses in authentication or application input handling could result in unauthorized access.

### Evidence

Screenshots and relevant findings are available in:

```text
M1-Initial-Access/
```

---

## 🔹 M2 – Data Extraction / Exposure

### Focus

* Application data-access testing
* Sensitive information exposure
* Authorization-boundary testing
* Data-access validation
* Evidence collection

### Objective

Determine whether application weaknesses could expose information outside the intended authorization boundary.

> 🔒 Sensitive patient information has been redacted and is not included in this public repository.

### Evidence

```text
M2-Data-Extraction/
```

---

## 🔹 M3 – Database Security Assessment

### Focus

* Database exposure assessment
* Database artifact analysis
* Backup exposure assessment
* Database structure review
* Security-impact analysis

### Objective

Evaluate whether exposed database resources could result in unauthorized access to application data.

> 🔒 Database records, credentials, and other sensitive information are not published in this repository.

### Evidence

```text
M3-Database-Exposure/
```

---

## 🔹 M4 – Password & Hash Security Assessment

### Focus

* Hash-format identification
* Password-storage analysis
* Controlled password-recovery testing
* Password-strength evaluation
* Credential-security assessment

### Objective

Determine whether the password-protection mechanism provides adequate resistance against credential compromise.

> 🔒 Actual passwords and sensitive credential values are not included in this repository.

### Evidence

```text
M4-Password-Assessment/
```

---

# 🛠️ Tools & Technologies

| Tool / Technology        | Purpose                                             |
| ------------------------ | --------------------------------------------------- |
|  Burp Suite           | HTTP traffic inspection and web application testing |
|  Web Browser           | Application analysis and validation                 |
|  SQL Injection Testing | Database/input security assessment                  |
|  Hash Identification   | Identify password/hash formats                      |
|  John the Ripper       | Controlled password-recovery testing                |
|  Kali Linux            | Cybersecurity testing environment                   |
|  Screenshot Tools      | Evidence collection                                 |
|  Markdown              | Technical documentation                             |

---

# 📊 Risk Summary

| Finding                                  | Severity    | Potential Impact                    |
| ---------------------------------------- | ----------- | ----------------------------------- |
| Authentication / Access-Control Weakness | 🔴 High     | Unauthorized access                 |
| Sensitive Data Exposure                  | 🔴 Critical | Disclosure of sensitive information |
| Database Exposure                        | 🔴 Critical | Database compromise                 |
| Weak Password / Hash Protection          | 🔴 High     | Credential compromise               |

---

# 🔍 Key Security Observations

### 1. Authentication Security

* Authentication should be enforced server-side.
* Strong authorization controls should be implemented.
* Authentication failures should be monitored.
* Rate limiting should be implemented.
* MFA should be considered for sensitive accounts.

### 2. Sensitive Data Protection

* Sensitive information should only be accessible to authorized users.
* Application responses should minimize unnecessary data exposure.
* Proper authorization checks should be applied to every protected resource.

### 3. Database Security

* Database backups should never be publicly accessible.
* Database permissions should follow the principle of least privilege.
* Exposed credentials should be rotated immediately.
* Database access should be restricted to trusted services.

### 4. Password Security

* Passwords should never be stored in plaintext.
* Strong adaptive password-hashing algorithms should be used.
* Unique salts should be used.
* Strong password policies should be enforced.
* MFA should be implemented for privileged accounts.

---

# 🛡️ Recommendations

## Authentication

* Implement secure server-side authentication.
* Enforce proper authorization checks.
* Implement login rate limiting.
* Enable MFA for sensitive accounts.
* Monitor repeated authentication failures.

## Database

* Remove database backups from public directories.
* Restrict database permissions.
* Rotate exposed credentials.
* Regularly audit backup locations.
* Apply network-level database restrictions.

## Password Security

* Use modern adaptive password hashing.
* Use unique salts for password hashes.
* Enforce appropriate password policies.
* Implement MFA.
* Monitor suspicious authentication activity.

## Web Application

* Use parameterized queries/prepared statements.
* Validate and sanitize server-side input.
* Implement proper access control.
* Follow the principle of least privilege.
* Keep software and dependencies updated.
* Conduct regular vulnerability assessments.

---

# 📁 Repository Structure

```text
Mediroza-Security-Assessment/
│
├── README.md
├── REPORT.md
│
├── All-Screenshots/
│
├── M1-Initial-Access/
│   ├── screenshots/
│   └── notes.md
│
├── M2-Data-Extraction/
│   ├── screenshots/
│   └── notes.md
│
├── M3-Database-Exposure/
│   ├── screenshots/
│   └── notes.md
│
├── M4-Password-Assessment/
│   ├── screenshots/
│   └── notes.md
│
└── Documentation/
    └── Final-Report.pdf
```

---

# 📄 Documentation

The complete assessment documentation contains:

* Introduction
* Scope and Rules of Engagement
* Assessment Methodology
* Tools Used
* M1 – Initial Access
* M2 – Data Extraction
* M3 – Database Security
* M4 – Password & Hash Assessment
* Evidence
* Risk Assessment
* Security Recommendations
* Conclusion

---

# 📸 Evidence

Screenshots and supporting evidence are organized according to each assessment milestone.

```text
All-Screenshots/
│
├── M1/
├── M2/
├── M3/
└── M4/
```

> ⚠️ Sensitive information, credentials, patient information, tokens, and other confidential data should be redacted before uploading screenshots to a public repository.

---

# ⚠️ Disclaimer

This repository is intended **only for authorized cybersecurity education, research, and security assessment**.

Do not use the techniques, tools, or information contained in this project against systems without explicit authorization.

Sensitive information has been redacted or omitted from the public documentation.

The author assumes no responsibility for unauthorized or illegal use of the information contained in this repository.

---

# 👤 Author

**Rashif K**

Cybersecurity Student
NETWORKWALKS – Batch B082

### Project

**Week 4 – Mediroza Hospital Security Assessment**

---

# Project Classification

```text
Category     : Cybersecurity
Project      : Security Assessment
Environment  : Authorized Lab
Batch        : B082
Week         : 4
Focus        : Web Application Security
```

---

⭐ **Educational cybersecurity project created for practical security-assessment training.**
