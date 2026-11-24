# URL & IOC Analysis

**Case ID:** PHISH-001

## Extracted Indicators

| IOC Type | Value | Assessment |
|---|---|---|
| Sender Email | support@company-helpdesk.example | Suspicious in this scenario |
| Sender Domain | company-helpdesk.example | Unverified |
| Return-Path | bounce@company-helpdesk.example | Recorded |
| URL | https://account-verification.example/login | Suspicious in context |
| URL Domain | account-verification.example | Fictional |
| IP Address | Not available | Not investigated |

## URL Investigation

- Protocol: HTTPS
- Domain: account-verification.example
- Path: /login
- Purpose: Requests account verification
- Authentication results: SPF fail, DKIM none, DMARC fail (simulated)

## Findings

1. The email creates urgency by threatening account suspension.
2. The URL requests immediate account verification.
3. The verification domain differs from the recipient's organizational domain.
4. The simulated email authentication results indicate failed SPF and DMARC checks.
5. The URL uses a reserved .example domain, so no live website or malicious infrastructure was verified.

## Assessment

**Verdict: Likely Phishing — Simulated Training Scenario**

The email contains multiple social engineering indicators. No real-world malicious activity has been confirmed.