# elevatelabstask13
Findings
🔴 Finding 1: Broken Object Level Authorization

Endpoint: GET /api/users/{id}

Issue: User ID manipulation allowed access to other user data.

Risk Level: High

OWASP Mapping: API1 – Broken Object Level Authorization

🟠 Finding 2: No Rate Limiting

Endpoint: POST /api/login

Issue: Unlimited login attempts allowed.

Risk Level: Medium

OWASP Mapping: API4 – Unrestricted Resource Consumption

🟡 Finding 3: Detailed Error Messages

Endpoint: /api/register

Issue: Server returned stack trace.

Risk Level: Low

OWASP Mapping: API8 – Security Misconfiguration

5️⃣ Recommendations

Implement role-based access control (RBAC)

Enforce JWT validation on all protected endpoints

Implement rate limiting (5 attempts per minute)

Disable verbose error messages in production

Validate all user inputs server-side
