Mediroza Hospital — Web Application Penetration Testing

About the Project

An authorized black-box web application penetration testing assessment conducted as part of a cybersecurity training engagement through Networkwalks Cybersecurity Lab.

The assessment focused on identifying vulnerabilities related to authentication, input validation, document security, metadata exposure, directory configuration, and backup security.

Target: Mediroza Hospital Web Application
Assessment Type: Authorized Black-Box Penetration Test
Environment: Educational / Training Lab

---

Objectives

- Assess the security of the authentication mechanism
- Identify input validation vulnerabilities
- Test for SQL injection
- Evaluate access controls for protected documents
- Analyse PDF password security
- Identify sensitive information in document metadata
- Detect exposed directories and legacy files
- Identify publicly accessible backup files
- Document security risks and remediation steps

---

Security Testing Performed

🔹 Reconnaissance

- Reviewed "robots.txt"
- Identified application paths
- Investigated legacy directories

🔹 Authentication Testing

- Tested username enumeration
- Analysed login responses
- Tested for SQL injection
- Verified authentication bypass in the authorized environment

🔹 Document Security

- Tested access to protected patient reports
- Analysed PDF encryption
- Performed authorized password recovery testing

🔹 Metadata Analysis

- Analysed PDF metadata using ExifTool
- Identified internal information exposed through document metadata

🔹 Backup & Directory Security

- Investigated legacy directories
- Identified directory listing misconfiguration
- Discovered an exposed database backup
- Assessed the potential impact of exposed information

---

Findings Summary

Severity| Findings
🔴 Critical| SQL Injection Authentication Bypass
🔴 Critical| Forgotten Backup Directory & Directory Listing
🔴 Critical| Confidential Data Exposure
🟠 High| Protected PDF Reports Accessible After Login Bypass
🟠 High| Weak PDF Password Protection
🟡 Medium| Username Enumeration
🟡 Medium| Sensitive PDF Metadata Exposure

The assessment identified 7 security findings across authentication, document protection, metadata handling, and backup exposure.

---

Tools Used

Kali Linux
cURL
John the Ripper
qpdf
ExifTool
grep
sed
wget
Web Browser

---

Key Security Recommendations

- Implement parameterized queries and prepared statements
- Apply proper server-side authorization
- Use strong and unique document passwords
- Remove unnecessary metadata from sensitive documents
- Disable directory listing
- Remove obsolete files and backups from public directories
- Store backups outside the web root
- Restrict backup access using proper authentication
- Encrypt sensitive backups
- Regularly audit web-accessible files and directories

---

Report

The complete assessment documentation is available in:

"Mediroza_Hospital_Pentest_Report.pdf"

---

Disclaimer

This project was performed as an authorized educational security assessment within a defined testing scope.

The techniques and tools documented here are intended for authorized penetration testing, cybersecurity learning, and defensive security research only.

Unauthorized testing of systems or applications is not permitted.

---

Author

V. Subhaharini

B.Sc. Computer Science with Cyber Security
Hindusthan College of Arts and Science

Training: Networkwalks Cybersecurity Lab
