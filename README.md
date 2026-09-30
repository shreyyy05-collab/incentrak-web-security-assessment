# IncenTrak Web Application Security Assessment

A portfolio case study documenting an authorized web application security assessment and remediation-validation workflow performed with OWASP ZAP and manual verification techniques.

> **Portfolio note:** This repository intentionally excludes credentials, session data, sensitive application endpoints, proprietary source code, and exploit-ready details. Findings are presented at a defensive, sanitized level.

## Project Overview

The purpose of this assessment was to identify web application security weaknesses, document their potential impact, communicate remediation priorities, and validate security improvements after changes were introduced.

Rather than treating vulnerability scanning as a one-time activity, the work followed an iterative security-testing lifecycle:

**Baseline Assessment → Findings Review → Remediation → Reassessment → Validation**

## My Role

- Configured OWASP ZAP for web application traffic inspection and security testing.
- Captured and reviewed application requests and responses through an intercepting proxy.
- Performed vulnerability analysis and manual validation where appropriate.
- Reviewed security-related HTTP response headers and common web security controls.
- Documented findings with their security relevance and remediation guidance.
- Reassessed the application after fixes to determine whether previously identified weaknesses remained.
- Compared assessment results across testing iterations to track remediation progress.

## Tools & Skills

- **OWASP ZAP**
- Web application security testing
- HTTP/HTTPS traffic analysis
- Vulnerability assessment
- Manual security validation
- Security header analysis
- Remediation verification
- Technical security reporting

## Assessment Areas

The assessment included review of common web application security concerns such as:

- Content Security Policy (CSP)
- HTTP Strict Transport Security (HSTS)
- X-Content-Type-Options
- Clickjacking protections
- Input-handling and injection-related testing
- Application responses and security-relevant HTTP behavior
- Scanner findings requiring manual review and validation

## Methodology

### 1. Baseline Assessment
Established an initial view of the application's security posture using OWASP ZAP and manual review.

### 2. Findings Analysis
Reviewed generated alerts to distinguish meaningful security concerns from items requiring additional validation.

### 3. Remediation Communication
Documented security weaknesses, their potential impact, and recommended defensive improvements.

### 4. Reassessment
Repeated testing after application changes to determine whether identified controls had been implemented or improved.

### 5. Validation
Compared subsequent results against earlier observations and documented remaining security concerns.

## Current Assessment Status

A newer validation assessment was performed on **September 29, 2026**. The latest report is being reviewed and sanitized before detailed results are published in this portfolio repository.

This prevents older assessment data from being represented as the application's current security state.

## Security Controls Reviewed

| Control | Security Purpose |
| --- | --- |
| Content Security Policy | Helps restrict which resources a browser is allowed to load and can reduce the impact of certain client-side injection attacks. |
| HTTP Strict Transport Security | Instructs supported browsers to use HTTPS for subsequent connections, reducing exposure to protocol-downgrade scenarios. |
| X-Content-Type-Options | Helps prevent browsers from interpreting resources as an unexpected MIME type. |
| Clickjacking Protection | Helps prevent application pages from being embedded in unauthorized frames or iframes. |

## Repository Structure

```text
incentrak-web-security-assessment/
├── README.md
├── docs/
│   ├── methodology.md
│   └── remediation-validation.md
└── evidence/
    └── README.md
```

Raw authenticated scan exports and sensitive application evidence are intentionally not published.

## What This Project Demonstrates

This project demonstrates practical experience with the security assessment lifecycle rather than scanner execution alone: configuring testing tools, inspecting web traffic, interpreting findings, validating controls, documenting risk, communicating remediation needs, and retesting after fixes.

## Responsible Disclosure & Confidentiality

This repository is a sanitized professional portfolio case study. It is not intended to disclose exploitable information about a production system. Sensitive URLs, authentication material, session information, customer or business data, proprietary implementation details, and other confidential information are excluded.

## Next Steps

The September 29, 2026 reassessment will be incorporated after the latest ZAP report is reviewed and sanitized. The results section will then document verified remediation progress and remaining findings without exposing sensitive application details.
