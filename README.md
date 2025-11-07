# OTP-BYPASS
This project demonstrates how One-Time Password (OTP) verification can be bypassed in vulnerable web applications using Burp Suite. It highlights common flaws in OTP implementation and emphasizes the importance of secure server-side validation.

# ⚙️ Tools & Environment
Operating System: Kali Linux

Proxy Tool: Burp Suite

Browser: Firefox/Chrome with proxy configured

Target: Vulnerable web application (e.g., sandbox or test site)

# 🚀 Steps to Reproduce
Launch Burp Suite and configure browser proxy settings.

Intercept the OTP submission request.

Modify request parameters (e.g., isVerified=true, reuse OTP, or skip OTP field).

Forward the manipulated request and observe server response.

Analyze whether authentication is bypassed.

# 🔍 Key Concepts
Intercepting and modifying HTTP requests

Client-side vs server-side validation

OTP reuse and logic flaws

Ethical penetration testing
