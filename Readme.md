🛡️ Web Application Security Testing – Task 1

Internship Program: Future Interns – Cyber Security
Intern Name: Priya Dharshini L
Task Code: FUTURE_CS_01

📌 Task Objective

The objective of this task is to perform security testing on a web application to identify common vulnerabilities such as:

SQL Injection

Cross-Site Scripting (XSS)

CSRF (Cross-Site Request Forgery)

Security misconfigurations

🌐 Target Application

The testing was performed on the following intentionally vulnerable web application:

http://testphp.vulnweb.com


This website is designed for legal and ethical penetration testing practice.

🛠 Tools Used

OWASP ZAP – Web application vulnerability scanner

Web Browser (Chrome) – For manual testing

🔍 Vulnerabilities Identified
Vulnerability	Risk Level
SQL Injection (MySQL & SQLite)	High
Cross-Site Scripting (XSS)	High
Missing CSRF Protection	Medium
Sensitive File Exposure (phpinfo)	Medium
Directory Browsing Enabled	Medium
Security Header Issues (CSP, Clickjacking, HSTS)	Medium/Low
🧪 Example Findings

SQL Injection

http://testphp.vulnweb.com/listproducts.php?cat='


This returned a database error, proving SQL injection vulnerability.

XSS

<script>alert(1)</script>


This payload executed JavaScript inside the user’s browser.

📄 Deliverables in This Repository

This repository contains:

Task1-Security-Report.docx – Detailed vulnerability report

Report of zap.pdf – Automated OWASP ZAP scan report

README.md – Task summary

🔐 Security Recommendations

Use prepared statements and parameterized queries

Validate and sanitize all user inputs

Implement CSRF tokens

Enable Content Security Policy (CSP)

Disable directory listing

Protect sensitive files like phpinfo.php

✅ Conclusion

The security assessment successfully identified critical vulnerabilities in the web application. These issues could lead to data breaches, account hijacking, and system compromise if not fixed. Proper security controls must be implemented to protect the application.

