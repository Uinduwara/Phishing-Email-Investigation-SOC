# SOC Phishing Email Investigation Report

**Case ID:** PHISH-001  
**Investigation Date:** 24 November 2026  
**Analyst:** SOC Analyst Trainee  
**Incident Category:** Suspected Credential Phishing  
**Classification:** Likely Phishing — Simulated Scenario  
**Case Status:** Analysis Completed

---

## 1. Executive Summary

This investigation examined a fictional suspicious email impersonating an IT Support team. The message pressured the recipient to verify their account within 24 hours to avoid account suspension.

Analysis identified multiple phishing indicators, including urgency-based social engineering, an unverified sender domain, a verification link, and simulated email authentication failures.

**Final Assessment:** Likely Phishing within the training scenario.

## 2. Email Details

| Field | Value |
|---|---|
| Sender | support@company-helpdesk.example |
| Recipient | employee@company.example |
| Subject | URGENT: Your Account Will Be Suspended |
| Return-Path | bounce@company-helpdesk.example |
| URL | https://account-verification.example/login |
| Attachment | None in sample |

## 3. Email Header Analysis

| Authentication | Result |
|---|---|
| SPF | Fail |
| DKIM | None |
| DMARC | Fail |

These authentication results were created for training purposes and do not represent actual mail-server verification.

## 4. IOC Analysis

The following indicators were extracted from the training email:

- Sender Domain: company-helpdesk.example
- Verification Domain: account-verification.example
- Suspicious URL: https://account-verification.example/login
- IP Address: Not available

All domains use the reserved `.example` namespace. No live malicious infrastructure was investigated.

## 5. Key Findings

1. The sender claims to represent the organization's IT Support team.
2. The email creates urgency through a 24-hour account suspension warning.
3. The verification URL uses a domain different from the recipient organization's domain.
4. The simulated authentication results show SPF and DMARC failures.
5. The message requests account verification through an external link.

## 6. Recommended SOC Actions

1. Advise the recipient not to click the link or enter credentials.
2. Preserve the email and its original headers.
3. Report the suspicious message to the security team.
4. Search authorized email logs for similar messages.
5. Verify whether any recipients interacted with the message.
6. Apply containment measures if an actual malicious threat is confirmed.
7. Document findings and escalate according to incident response procedures.

## 7. Evidence Collected

| Evidence ID | Description |
|---|---|
| Evidence 01 | Suspicious Email Overview |
| Evidence 02 | Email Header Analysis |
| Evidence 03 | Sender and Domain Investigation |
| Evidence 04 | URL and IOC Analysis |
| Evidence 05 | Final Verdict and SOC Recommendations |

## 8. Conclusion

The fictional email demonstrated several common characteristics of credential phishing, including impersonation, urgency, and account verification requests.

Based on the simulated evidence, the message was classified as likely phishing.

This investigation was performed entirely within a training scenario. No real phishing infrastructure was contacted, and no actual security incident was confirmed.

---

**Report Type:** SOC Analyst Portfolio Project  
**Environment:** Simulated Training Lab