# Brute Force Alert Triage (SOC Tier 1)

## Purpose
This document captures the Tier 1 SOC analyst triage process for a suspected brute force authentication attempt.

## Alert Overview
- Alert Type: Excessive Failed Authentication Attempts
- Detection Source: Authentication Logs / SIEM
- Initial Severity: Medium
- Potential Risk: Account compromise

## Evidence Reviewed
- Authentication log sample (Logs/auth_sample.log)
- Terminal-based log analysis

## Tier 1 Triage Steps
1. Reviewed volume of failed authentication attempts
2. Identified source IP address
3. Identified targeted user account(s)
4. Checked for any successful login following failures
5. Determined likelihood of brute force behavior
6. Documented findings and escalation decision

## Findings
- Multiple failed login attempts within a short time window
- Single external IP address responsible for all attempts
- Targeted account: admin
- No successful authentication observed

## Disposition
- Classification: True Positive (Brute Force Attempt)
- Account Compromise: Not confirmed
- Escalation Required: Yes (Tier 2)

## Tier 1 Actions Taken
- Alert validated
- Source IP identified and documented
- Findings escalated for blocking and further monitoring

## MITRE ATT&CK Mapping
- T1110 – Brute Force
