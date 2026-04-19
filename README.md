🔐 API Security Risk Analysis (Modern SaaS Skill)

📌 Overview

This project presents a hands-on API Security Testing Report conducted using Postman on Kali Linux.
The goal was to simulate a real-world security analysis by thinking like an attacker and identifying vulnerabilities in a public API.

🎯 Objective
 • Understand how APIs work
 • Identify common API security vulnerabilities
 • Analyze risks and their impact
 • Provide recommendations to secure APIs

🛠️ Tools & Environment
 • Tool Used: Postman
 • Operating System: Kali Linux
 • API Tested: JSONPlaceholder
 • Base URL: https://jsonplaceholder.typicode.com

🧪 Testing Methodology

The following steps were performed during testing:
 1. Sent requests to retrieve public user data
 2. Manipulated URL parameters manually
 3. Tested API responses with different inputs
 4. Attempted to send and create user data
 5. Analyzed server responses for vulnerabilities

🔍 Key Findings

1. ❌ No Authentication
 • API allowed access without login credentials
 • Anyone can retrieve user data

Risk Level: Medium to High

2. 🔓 Broken Authorization
 • Changing user IDs in the URL exposed different user data
 • No access control mechanism

Risk Level: Medium to High

3. 📤 Excessive Data Exposure
 • API returned sensitive data such as:
 • Email
 • Phone number
 • Address

Risk Level: Medium to High

4. ⚠️ Lack of Input Validation
 • Invalid requests returned empty responses instead of errors
 • Indicates weak validation

Risk Level: Medium to High

5. 🧾 Unrestricted Data Creation
 • API accepted fake user data without validation
 • No authentication required

Risk Level: Medium to High

📊 Conclusion

This API demonstrates several critical security weaknesses:
 • No authentication or authorization
 • Exposure of sensitive data
 • Weak input validation
 • Open data creation

⚠️ In a real-world system, these issues could lead to:
 • Data breaches
 • Identity impersonation
 • System abuse and spam

✅ Recommendations

1. Add Authentication
 • Use API keys or tokens
 • Deny access without valid credentials

2. Enforce Authorization
 • Ensure users can only access their own data

3. Limit Data Exposure
 • Return only necessary information

4. Validate Inputs
 • Check all incoming data for correctness and security

5. Improve Error Handling
 • Provide meaningful errors without exposing system details

📚 Notes
 • The API used (JSONPlaceholder) is a mock API for learning purposes
 • No real user data was involved
 • All testing was conducted ethically and safely

👨‍💻 Author

Temen Alemayehu
API Security Analysis Project – 2026
