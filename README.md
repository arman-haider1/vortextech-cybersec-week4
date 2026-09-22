# VORTEXTECH Cyber Security Internship — Week 4

## Mini Incident Response Plan

**Track:** Advanced  
**Task:** Week 4 of 4  
**Project Type:** Incident Response & Cybersecurity Documentation  
**Scenario:** Hypothetical Customer Data Breach  
**Framework:** NIST Incident Response Lifecycle

---

## 📌 Project Overview

This project was completed as part of the **VORTEXTECH Cyber Security Internship — Week 4 Advanced Track**.

The project presents a structured **Mini Incident Response Plan** for a fictional e-commerce company named **NovaCart**. The scenario focuses on a customer-facing API endpoint that was incorrectly configured and failed to enforce proper server-side authorization.

As a result, an unauthorized user could potentially retrieve records belonging to other customers by modifying an identifier in an API request.

The incident response plan demonstrates how a security team would prepare for, detect, contain, eradicate, recover from, and learn from such an incident.

The plan follows the **six-phase NIST Incident Response Lifecycle**:

1. Preparation
2. Detection & Analysis
3. Containment
4. Eradication
5. Recovery
6. Post-Incident Review / Lessons Learned

---

## 🎯 Objective

The objective of this project is to demonstrate the ability to develop a realistic and structured incident response plan for a hypothetical security breach.

The plan covers:

- A realistic breach scenario
- Incident discovery and analysis
- Potentially affected data
- Root-cause identification
- Incident response activities
- Internal communication procedures
- Recovery and post-incident activities
- Preventative security measures

---

## 🏢 Hypothetical Company

### NovaCart

NovaCart is a fictional online retail/e-commerce platform that stores customer account and order information.

The hypothetical incident involves an unsecured customer-facing API endpoint that does not properly enforce server-side authorization.

---

## 🚨 Breach Scenario

### Incident

A customer-facing API endpoint was misconfigured and failed to enforce server-side authorization.

An attacker could potentially retrieve another customer's records simply by modifying an identifier included in an API request.

### Discovery

The incident is identified through an automated monitoring alert reporting an unusually high volume of database queries originating from the customer API.

Security analysts then identify repeated requests attempting to access records outside the authenticated user's account.

### Data at Risk

The potentially exposed information includes:

- Customer names
- Email addresses
- Delivery addresses
- Order history
- Internal customer IDs

Payment-card details are excluded from this scenario because they are handled by a separate payment provider.

### Root Cause

The identified root causes are:

- Missing server-side authorization checks
- Insufficient security testing of the API endpoint before deployment

---

# 🔐 Incident Response Framework

The response plan follows the six phases of the **NIST Incident Response Lifecycle**.

## 1. Preparation

Preparation focuses on security capabilities that should already exist before an incident occurs.

NovaCart should maintain:

- A designated Incident Response Team (IRT)
- Clearly defined incident-response roles and contact information
- Centralized logging
- Security monitoring and automated alerting
- Documented response procedures
- Asset inventories
- Access-control policies
- Regular and securely stored backups
- Periodic API and web-service security testing
- Specific testing for broken access-control conditions

---

## 2. Detection & Analysis

The incident is detected through an automated alert indicating abnormal database-query activity from the customer API.

The security team would:

1. Validate the alert.
2. Determine whether the alert is a false positive.
3. Identify the affected API endpoint.
4. Review API and database logs.
5. Establish the timeframe of suspicious activity.
6. Identify potentially affected customer accounts or records.
7. Preserve relevant logs and forensic evidence in an unaltered state.
8. Determine the scope and impact of the incident.

---

## 3. Containment

The containment phase focuses on preventing additional unauthorized access.

Actions include:

- Restricting access to the affected API endpoint
- Temporarily disabling the endpoint if necessary
- Revoking or rotating associated API keys
- Revoking or rotating session tokens and credentials
- Isolating affected servers or services where required
- Increasing monitoring across related systems
- Documenting containment actions, timestamps, and personnel involved

---

## 4. Eradication

Eradication removes the underlying cause of the incident.

The response team would:

- Correct the API's server-side authorization logic.
- Ensure every request is validated against the authenticated user's permissions.
- Verify resource ownership before returning customer information.
- Remove unauthorized access mechanisms.
- Remove suspicious credentials or malicious configuration changes identified during investigation.
- Perform thorough security testing of the corrected endpoint before returning it to service.

---

## 5. Recovery

Recovery focuses on safely restoring normal operations.

The corrected API endpoint would be redeployed in a controlled and phased manner.

The team would then:

- Verify that authorization checks function correctly.
- Test the corrected service under realistic conditions.
- Review and confirm system integrity.
- Gradually restore normal traffic.
- Maintain enhanced monitoring after restoration.
- Confirm that there are no continuing signs of unauthorized access.

Recovery is considered complete only after normal operation has been confirmed.

---

## 6. Post-Incident Review / Lessons Learned

After recovery, NovaCart would conduct a formal post-incident review.

The review would document:

- The complete incident timeline
- Affected systems and data
- Detection and response actions
- Confirmed root cause
- Gaps in API authorization
- Security-testing weaknesses
- Logging and monitoring gaps
- Corrective actions
- Responsible teams
- Priorities and follow-up deadlines

The incident response plan would then be updated based on the lessons learned from the incident.

---

# 📢 Internal Communication Plan

| Timing | Audience | Purpose |
|---|---|---|
| Immediately after alert validation | Security / Incident Response Team & Internal Leadership | Confirm the incident, assign ownership, and coordinate the initial response. |
| During initial investigation | Legal / Compliance & Technical Owners | Discuss the incident's nature, scope, available evidence, and applicable response obligations. |
| After impact is established | Affected Customers, where applicable | Provide clear factual information and relevant protective steps. |
| As required by applicable law | Relevant Regulators / Authorities | Submit required incident notifications through the appropriate regulatory process. |

---

# 🛡️ Preventative Measures

## 1. Enforce Server-Side Authorization

Every API request should verify:

- Authentication
- Authorization
- Resource ownership

Authorization must be enforced on the server and should not rely solely on client-supplied identifiers.

## 2. Conduct Regular API Security Testing

Customer-facing APIs should be tested before deployment and periodically afterward.

Testing should specifically include broken-access-control scenarios and attempts to access resources belonging to other users.

## 3. Improve Monitoring and Alerting

Centralized API and database logging should detect abnormal access patterns, including:

- Unusually high query volumes
- Cross-account record access
- Other anomalous API activity

Timely alerts should be generated for security-team investigation.

---

# 📄 Project Deliverable

The main deliverable is the **Mini Incident Response Plan** document containing the complete hypothetical incident scenario, six-phase response process, communication plan, preventative measures, and conclusion.

**PDF filename:** `VortexTech_Week4_Incident_Response_Plan.pdf`

---

# 🧰 Technologies / Concepts

This project focuses primarily on cybersecurity incident-response concepts rather than implementation of a software application.

### Key Concepts

- Incident Response
- NIST Incident Response Lifecycle
- Security Monitoring
- Log Analysis
- API Security
- Server-Side Authorization
- Access Control
- Incident Containment
- Incident Eradication
- System Recovery
- Post-Incident Review
- Security Preventative Measures

---

# 📁 Repository Structure

```text
vortextech-cybersec-week4/
│
├── README.md
│
└── VortexTech_Week4_Incident_Response_Plan.pdf
```

---

# 🎓 Internship Context

**Program:** VORTEXTECH Cyber Security Internship 2026  
**Week:** 4 of 4  
**Track:** Advanced  
**Task:** Mini Incident Response Plan

This project demonstrates the application of structured incident-response principles to a realistic hypothetical customer-data breach scenario.

---

## ⚠️ Disclaimer

This project uses a **fictional company and hypothetical breach scenario** created for cybersecurity education and internship assessment purposes.

No real organization, customer database, or production system was targeted.

---

## 👤 Author

**Arman Haider**  
Cyber Security Intern

**VORTEXTECH Cyber Security Internship — Week 4 Advanced**
