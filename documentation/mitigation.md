# Vulnerability Mitigation Recommendations

## 01 / Stored Cross-Site Scripting (XSS)

### Identified Weaknesses

- Improper handling of untrusted user input.
- Direct rendering of stored content.
- Missing output encoding.

### Recommended Security Controls

- Validate user input on the server side.
- Apply context-appropriate output encoding.
- Sanitize untrusted HTML content.
- Implement Content Security Policy (CSP).
- Configure HttpOnly and Secure cookie attributes.

## 02 / Cross-Site Request Forgery (CSRF)

### Identified Weaknesses

- Missing anti-CSRF tokens.
- Insufficient request origin verification.
- Missing re-authentication for sensitive actions.

### Recommended Security Controls

- Implement anti-CSRF tokens.
- Configure SameSite cookie attributes.
- Validate request origins.
- Require re-authentication for sensitive operations.
- Avoid GET requests for state-changing operations.

## 03 / Security Recommendations

- Conduct regular vulnerability assessments.
- Follow OWASP secure coding guidelines.
- Perform security testing throughout the development lifecycle.
- Verify security controls through post-mitigation testing.

## 04 / Documentation Note

These mitigation techniques were proposed based on the vulnerabilities demonstrated during the academic project.

The recommended controls were not implemented or independently tested during the original project.
