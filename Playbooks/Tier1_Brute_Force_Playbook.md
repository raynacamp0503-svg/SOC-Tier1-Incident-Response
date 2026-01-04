# Tier 1 Playbook — Brute Force Authentication Attempts

## Purpose
Standardize Tier 1 analysis and escalation of brute force or password spray authentication alerts.

## Scope
- SOC Tier 1 analysts
- SSH, RDP, VPN, or directory authentication failures

## Alert Sources
- Authentication logs
- SIEM correlation alerts
- Endpoint or network security tools

## Tier 1 Responsibilities
- Validate alert volume and timeframe
- Identify source IP(s)
- Identify targeted account(s)
- Determine whether authentication succeeded
- Document findings and escalate when necessary

## Tier 1 Investigation Steps
1. Count failed authentication attempts
2. Identify the timeframe of activity
3. Identify source IP address(es)
4. Identify targeted account(s)
5. Check for successful logins following failures
6. Determine whether activity matches brute force or password spray behavior
7. Document findings in the alert triage document

## Escalation Criteria (Tier 2)
Escalate immediately if any of the following are true:
- Successful login occurred after failures
- Privileged or admin account targeted
- Multiple accounts targeted from same IP
- Activity observed across multiple systems
- Repeated activity from same source over time

## Tier 1 Containment Actions (If Authorized)
- Recommend blocking source IP
- Recommend password reset if compromise suspected
- Verify MFA and account lockout policies

## References
- MITRE ATT&CK: T1110 – Brute Force
- NIST Incident Response Lifecycle
