# Phishing Alert Triage (SOC Tier 1)

## Purpose
This document captures the Tier 1 SOC analyst triage process for a phishing email alert.

## Alert Overview
- Alert Type: Phishing Email (Suspicious Link)
- Detection Source: Email Security Gateway / SIEM
- Initial Severity: Medium
- Potential Risk: Credential harvesting

## Tier 1 Triage Steps
1. Review alert details (timestamp, recipient, subject)
2. Verify sender email address and domain legitimacy
3. Analyze email headers for authentication failures (SPF, DKIM, DMARC)
4. Identify social engineering indicators (urgency, spoofing language)
5. Inspect embedded links without clicking
6. Determine whether the user interacted with the email
7. Document findings and determine disposition

## Findings
- Sender domain appears to be a look-alike domain (typosquatting)
- Email content uses urgency-based language
- Header authentication checks failed
- No evidence of user interaction observed

## Disposition
- Classification: True Positive (Phishing Attempt)
- User Compromise: Not confirmed
- Escalation Required: Yes (Tier 2 awareness)

## Tier 1 Actions Taken
- Alert validated
- Email recommended for quarantine
- Malicious sender domain recommended for blocking
- Findings documented for escalation

## MITRE ATT&CK Mapping
- T1566.002 – Phishing: Spearphishing Link

## Evidence Reviewed (Email Headers)
- Sender domain: paypa1.com (typosquatting)
- SPF: fail
- DKIM: none
- DMARC: fail
- Sending IP: 185.203.116.23

This evidence supports classification of the alert as a phishing attempt.
