# Tier 1 Playbook — Phishing Email

## Purpose
Provide a standardized Tier 1 response process for phishing email alerts to ensure consistent validation, documentation, and escalation.

## Scope
- SOC Tier 1 analysts
- Email-based phishing alerts
- No malware execution or deep forensics at this stage

## Alert Sources
- Email Security Gateway
- SIEM correlation rules
- User-reported suspicious emails

## Tier 1 Responsibilities
- Validate alert legitimacy
- Identify phishing indicators
- Determine user interaction status
- Document findings clearly
- Escalate when criteria are met

## Tier 1 Investigation Steps
1. Review alert metadata (timestamp, recipient, subject)
2. Validate sender address and domain
3. Review email headers (SPF, DKIM, DMARC)
4. Identify social engineering indicators (urgency, spoofing)
5. Extract IOCs (sender domain, IP, URLs)
6. Determine whether the user clicked links or opened attachments
7. Record findings in the alert triage document

## Escalation Criteria (Tier 2)
Escalate immediately if any of the following are true:
- User clicked a malicious link
- Credentials were entered
- Attachment was opened
- Multiple users were targeted
- Similar emails observed in a short timeframe

## Tier 1 Containment Actions (If Authorized)
- Quarantine email
- Block sender domain
- Block malicious URLs
- Notify affected user(s)

## References
- MITRE ATT&CK: T1566.002 – Phishing: Spearphishing Link
- NIST Incident Response Lifecycle
