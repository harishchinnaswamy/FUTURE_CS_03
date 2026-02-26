# FUTURE_CS_03
API SECURITY RISK ASSESSMENT REPORT
# Task 3 – API Security Risk Analysis (ReqRes API)

This repository contains a manual read-only API security assessment conducted on the ReqRes Demo API as part of Cyber Security Task 3.

The objective of this assessment was to evaluate authentication enforcement, access control mechanisms, HTTP method restrictions, and overall API security posture without performing exploitation or unauthorized access attempts.

---

## 📌 API Tested

- **API Name:** ReqRes Demo API  
- **Base URL:** https://reqres.in  
- **Assessment Type:** Manual Read-Only Security Evaluation  
- **Testing Tool:** Postman  

---

## 🎯 Scope of Assessment

### Included:
- Public demo endpoints
- GET request validation
- Safe method testing (POST, PUT, DELETE behavior analysis)
- Authorization header inspection
- Response and HTTP status code analysis
- Documentation-based review

### Excluded:
- Exploitation attempts
- Authentication bypass testing
- Denial-of-Service (DoS) testing
- Automated brute-force attempts
- Private or production API targeting

All testing was conducted within ethical and legal boundaries using only the public demo environment.

---

## 🛠 Tools Used

- **Postman** – API request testing and response inspection  
- **Browser Developer Tools** – Header and network inspection  
- **Manual Risk Classification** – Severity and likelihood assessment  

---

## 🔎 Methodology

The assessment was conducted in the following steps:

1. Reviewed official API documentation
2. Enumerated public endpoints
3. Tested access control enforcement
4. Validated HTTP method restrictions
5. Supplied invalid authentication headers
6. Observed response behavior and status codes
7. Classified risks based on severity and business impact

No exploitation or bypass techniques were performed.

---

## 🚨 Identified Risks

| Risk Area                     | Severity |
|------------------------------|----------|
| Public Base Endpoint Exposure | Low      |
| Access Control Enforcement    | Low      |
| HTTP Method Restrictions      | Low      |
| Authentication Validation     | Low      |
| Rate Limiting (Production)    | Medium   |

### Key Observations:
- Unauthorized requests were correctly denied (403 responses).
- Invalid authentication tokens were rejected.
- Method-level access controls prevented data modification.
- Rate limiting mechanisms were not observable during manual testing (conditional improvement recommended for production environments).

---

## 📊 Risk Methodology

Risk levels were assigned based on:

- Observed API behavior
- Potential exploitability
- Business impact in a real SaaS environment
- Likelihood of abuse in production scenarios

Severity Levels:
- **Low** – Minimal impact, properly controlled
- **Medium** – Improvement recommended for production
- **High** – Critical exposure (not observed in this assessment)

---

## 🛡 OWASP API Security Considerations

The assessment considered common OWASP API Security risk categories including:

- Broken Object Level Authorization
- Broken Authentication
- Excessive Data Exposure
- Security Misconfiguration
- Lack of Rate Limiting

No critical OWASP API violations were identified within the defined scope.

---

---

## 📌 Conclusion

Based on the read-only security testing performed, the ReqRes Demo API demonstrates proper access control enforcement and authentication validation.

No high-risk vulnerabilities were identified within scope.  
For production environments, rate limiting, monitoring, and centralized logging mechanisms are recommended to strengthen resilience against automated abuse.

---

**Author:** Harish C  
Cybersecurity Intern  
Future Interns
