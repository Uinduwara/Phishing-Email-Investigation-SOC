# Sender & Domain Investigation

**Case ID:** PHISH-001

**Sender:** support@company-helpdesk.example

**Sender Domain:** company-helpdesk.example

**Recipient:** employee@company.example

**Return-Path:** bounce@company-helpdesk.example

## Authentication Results

- SPF: Fail
- DKIM: None
- DMARC: Fail

## Suspicious Indicators

1. The email claims to be from IT Support.
2. The sender domain differs from the recipient's organizational domain.
3. The subject uses urgency and threatens account suspension.
4. The email requests immediate identity verification through a link.
5. The simulated email authentication results show SPF and DMARC failures.

## Preliminary Verdict

**Suspicious — Likely Phishing (Training Scenario)**

The email exhibits multiple phishing indicators. Additional verification would be required before confirming a real-world incident.

**Note:** All domains and authentication results are fictional training data.