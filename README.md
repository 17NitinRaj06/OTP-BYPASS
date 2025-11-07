# OTP-BYPASS
1. Objective

Demonstrate how OTP (One-Time Password) verification can be bypassed using Burp Suite.

Highlight vulnerabilities in poorly implemented OTP systems.

2. Tools Used

Kali Linux: Penetration testing OS.

Burp Suite: Web vulnerability scanner and proxy tool.

Optional: Web browser (e.g., Firefox), vulnerable web app for testing(https://www.bakingo.com/).

3. Setup

Launch Burp Suite and configure browser proxy settings.

Intercept traffic between browser and server using Burp Suite.

4. Target Scenario

A web application that sends OTP to user’s phone/email for login or transaction verification.

OTP is entered in a form and submitted to the server for validation.

5. Attack Method

Intercept the OTP submission request using Burp Suite.

Modify or replay the request:

Bypass via Response Manipulation: Change server response to simulate success.

Resend Same OTP: Exploit if OTP is not invalidated after first use.

Force Logical Flaws: Skip OTP validation by altering parameters (e.g., isVerified=true).

Brute Force or Predictable OTPs: Try common OTPs if rate limiting is weak.

6. Key Vulnerabilities Exploited

Lack of server-side OTP validation.

Reusable or predictable OTPs.

Missing rate limits or CAPTCHA.

Client-side trust (e.g., relying on frontend flags).

7. Outcome

Successful login or transaction without valid OTP.

Demonstrates critical flaw in authentication flow.
