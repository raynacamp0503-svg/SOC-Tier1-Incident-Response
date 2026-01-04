# Suspicious PowerShell Alert Triage (SOC Tier 1)

## Purpose
Document Tier 1 triage actions for alerts involving potentially malicious PowerShell execution.

## Alert Overview
- Alert Type: Suspicious PowerShell Command Execution
- Detection Source: Endpoint Logs / SIEM
- Initial Severity: Medium
- Potential Risk: Initial access, malware execution, or post-exploitation activity

## Evidence Reviewed
- PowerShell script block logging (Event ID 4104)
- Command-line parameters observed
- User and host context

## Tier 1 Triage Steps
1. Review PowerShell command-line arguments
2. Identify suspicious flags (encoded commands, hidden windows, bypass)
3. Identify user context and host
4. Determine whether activity aligns with normal administrative behavior
5. Document findings and escalate if necessary

## Findings
- PowerShell executed with encoded command (-enc)
- Use of -NoProfile and hidden window
- ExecutionPolicy bypass observed
- Activity not consistent with typical user behavior

## Disposition
- Classification: Suspicious Activity
- Malicious Activity: Not confirmed
- Escalation Required: Yes (Tier 2)

## Tier 1 Actions Taken
- Alert validated
- Suspicious command execution documented
- Escalated for further endpoint investigation

## MITRE ATT&CK Mapping
- T1059.001 – Command and Scripting Interpreter: PowerShell
