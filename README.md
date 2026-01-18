# FUTURE_CS_01
Cyber Security Task 1 – Web Application Security Testing
📌 Project Overview

This repository contains a web application security testing report conducted on OWASP Juice Shop, an intentionally vulnerable application developed for security training. The purpose of this task is to identify common web vulnerabilities, understand their impact, and recommend mitigation strategies using industry-standard security tools.

The assessment simulates a real-world penetration testing scenario and maps the findings to the OWASP Top 10 security risks.

🎯 Objectives

Perform basic web application security testing

Identify common vulnerabilities in a web application

Use professional security tools for testing

Understand the impact of vulnerabilities

Map findings to OWASP Top 10 categories

🧪 Test Application

OWASP Juice Shop

OWASP Juice Shop is a deliberately insecure web application that contains real-world security flaws. It is widely used for learning, practicing, and demonstrating web application security testing techniques.

🛠 Tools Used

OWASP ZAP (Zed Attack Proxy)
Used for automated scanning, intercepting HTTP requests, and identifying security weaknesses.

Burp Suite
Used for manual testing, request manipulation, and validation of discovered vulnerabilities.

🔍 Identified Vulnerabilities
1. SQL Injection

Description: Login page accepts malicious SQL input.

Screenshot Title: OWASP Juice Shop SQL Injection Login Page

Impact: High

OWASP Category: A03 – Injection

Explanation:
Improper input handling allows attackers to manipulate SQL queries, potentially bypassing authentication and accessing sensitive data.

2. Cross-Site Scripting (XSS)

Description: Script injected in the search field.

Screenshot Title: OWASP Juice Shop Reflected XSS Search

Impact: Medium

OWASP Category: A07 – Cross-Site Scripting (XSS)

Explanation:
The application reflects unsanitized user input back to the browser, allowing execution of malicious JavaScript code.

3. Broken Authentication

Description: Weak password allowed during login.

Screenshot Title: OWASP Juice Shop Weak Password Login

Impact: High

OWASP Category: A02 – Broken Authentication

Explanation:
Weak password enforcement increases the risk of brute-force and credential-stuffing attacks.

🛡 Mitigation Steps

Use prepared statements and parameterized queries to prevent SQL Injection

Validate, sanitize, and encode all user inputs to prevent XSS

Enforce strong password policies, account lockout mechanisms, and Multi-Factor Authentication (MFA)

📚 OWASP Top 10 Mapping

A02 – Broken Authentication

A03 – Injection

A07 – Cross-Site Scripting (XSS)

✅ Conclusion

This project demonstrates how common web application vulnerabilities can be identified using standard security tools. The findings highlight the importance of secure coding practices, proper input validation, and strong authentication mechanisms. This assessment reflects a realistic client-side security testing scenario.

⚠ Disclaimer

OWASP Juice Shop is an intentionally vulnerable application.
All testing was performed in a controlled environment for educational purposes only.
