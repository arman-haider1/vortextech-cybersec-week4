# VORTEXTECH Cyber Security Internship — Week 4

## Mini Incident Response Plan

**Track:** Advanced  
**Task:** Week 4 of 4  
**Project:** Mini Incident Response Plan  
**Scenario:** Hypothetical Customer Data Breach  
**Framework:** NIST Incident Response Lifecycle

## Overview

This project presents a structured incident response plan for **NovaCart**, a fictional e-commerce company. The hypothetical incident involves a customer-facing API endpoint that failed to enforce server-side authorization, potentially allowing unauthorized access to other customers' records.

The plan demonstrates how a security team would respond to the incident from initial preparation through post-incident review.

## Incident Scenario

- **Company:** NovaCart — fictional e-commerce platform
- **Incident:** Misconfigured API endpoint with missing server-side authorization
- **Discovery:** Automated monitoring detected unusual database-query activity
- **Data at Risk:** Customer names, email addresses, delivery addresses, order history, and internal customer IDs
- **Root Cause:** Missing server-side authorization checks and insufficient API security testing
- **Payment Data:** Excluded from the scenario because payment-card details are handled by a separate provider

## Incident Response Phases

The plan follows six phases of the NIST Incident Response Lifecycle:

1. **Preparation** — Establish response capabilities, monitoring, logging, backups, procedures, and security testing.
2. **Detection & Analysis** — Validate alerts, investigate logs, identify affected systems/data, and preserve evidence.
3. **Containment** — Restrict the affected API, revoke or rotate relevant credentials, isolate systems when required, and increase monitoring.
4. **Eradication** — Correct server-side authorization, remove unauthorized access mechanisms, and security-test the corrected endpoint.
5. **Recovery** — Restore the service in a controlled manner, verify authorization and system integrity, and maintain enhanced monitoring.
6. **Post-Incident Review / Lessons Learned** — Document the incident, identify security gaps, assign corrective actions, and update the response plan.

## Communication Plan

The response plan defines communication with:

- Security / Incident Response Team and internal leadership
- Legal / Compliance and technical owners
- Affected customers, where applicable
- Relevant regulators / authorities, as required by applicable law

## Preventative Measures

1. **Enforce server-side authorization** for authentication, authorization, and resource ownership.
2. **Conduct regular API security testing**, including broken-access-control scenarios.
3. **Improve monitoring and alerting** for anomalous API and database access patterns.

## Repository Contents

```text
vortextech-cybersec-week4/
├── README.md
└── VortexTech_Week4_Incident_Response_Plan.pdf
```

## Deliverable

The repository contains the complete **Mini Incident Response Plan** prepared for the VORTEXTECH Cyber Security Internship — Week 4 Advanced track.

**PDF:** `VortexTech_Week4_Incident_Response_Plan.pdf`

## Disclaimer

This project uses a fictional company and hypothetical breach scenario for cybersecurity education and internship assessment purposes. No real organization, customer database, or production system was targeted.

## Author

**Arman Haider**  
Cyber Security Intern

**VORTEXTECH Cyber Security Internship — Week 4 Advanced**

