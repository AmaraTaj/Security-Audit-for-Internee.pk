Security-Audit-for-Internee.pk
"Penetration testing project for Internee.pk using OWASP ZAP. Includes automated scans, manual testing for SQLi, XSS, and CSRF, and a professional report with findings and recommendations."

📌 Scope
- Assess the security of Internee.pk login system, user profiles, and APIs.
- Detect potential vulnerabilities such as:
  - SQL Injection (SQLi)
  - Cross-Site Scripting (XSS)
  - Cross-Site Request Forgery (CSRF)

📌 Methodology
- **Automated Scanning:** Performed with OWASP ZAP Active Scan.
- **Manual Testing:** Fuzzing requests with common payloads for SQLi and XSS.
- **CSRF Testing:** Replayed authentication requests without cookies to check token validation.
- **Header Review:** Verified security headers like `Strict-Transport-Security` and `X-Frame-Options`.

📌 Findings
- **SQL Injection:** No vulnerabilities detected.  
- **Cross-Site Scripting (XSS):** No vulnerabilities detected.  
- **Cross-Site Request Forgery (CSRF):**  
  - Potential vulnerability found on `POST /sign-in/factor-one` as the request returned `HTTP/1.1 200 OK` even when re-sent without cookies.  

📌 Deliverables
- Penetration Testing Report (DOCX/PDF) → Detailed methodology, findings, and recommendations.
- OWASP ZAP HTML Report → Generated report containing scan results and request/response logs.
- Screenshots → Evidence of ZAP scans, including the Alerts tab and CSRF test results.

📌 Tools Used
- [OWASP ZAP](https://www.zaproxy.org/)  
- Mozilla Firefox with FoxyProxy Extension  
- Windows 10 Environment  

📌 Author
**Amara Taj**  
Intern at Internee.pk  

