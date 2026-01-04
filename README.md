# SOC Tier 1 Incident Response Portfolio

This repository demonstrates hands-on SOC Tier 1 analyst skills through realistic alert triage scenarios, evidence-based analysis, and standardized response playbooks.

The project focuses on how a Tier 1 analyst validates alerts, analyzes logs, documents findings, and escalates incidents following established SOC processes.

---

## SOC Tier 1 Scenarios Covered

### 1. Phishing Email Alert
- Analyzed suspicious email headers (SPF, DKIM, DMARC)
- Identified typosquatted sender domain and social engineering indicators
- Determined true positive phishing attempt
- Documented findings and escalated to Tier 2

**MITRE ATT&CK:** T1566.002 – Phishing: Spearphishing Link

---

### 2. Brute Force Authentication Attempt
- Analyzed authentication logs using command-line tools
- Identified repeated failed login attempts from a single external IP
- Confirmed brute force behavior targeting an admin account
- Documented incident and escalated for blocking and monitoring

**MITRE ATT&CK:** T1110 – Brute Force

---

### 3. Suspicious PowerShell Execution
- Reviewed endpoint PowerShell execution logs (Event ID 4104)
- Identified suspicious flags including encoded commands and execution policy bypass
- Assessed user and host context
- Escalated activity for deeper endpoint investigation

**MITRE ATT&CK:** T1059.001 – Command and Scripting Interpreter: PowerShell

---

## Skills Demonstrated

- SOC Tier 1 alert triage and validation
- Log analysis using PowerShell and command-line tools
- Phishing and social engineering detection
- Authentication and endpoint behavior analysis
- Evidence-based incident documentation
- Escalation decision-making
- Following SOC playbooks and runbooks

---

## Tools and Concepts

- Git & GitHub (version control and documentation)
- Windows PowerShell
- Command-line log analysis
- Email header analysis
- SIEM alert concepts
- MITRE ATT&CK framework
- NIST Incident Response lifecycle

---

## Scope Note

This project is intentionally scoped to **SOC Tier 1 responsibilities**.  
Advanced forensics, malware reverse engineering, and threat hunting are outside the scope of this portfolio.

---

## Repository Structure

- Alert-Triage/ — Tier 1 alert investigation documentation  
- Playbooks/ — Standardized Tier 1 response playbooks  
- Logs/ — Sample log data used for analysis  
- Incident-Reports/ — Incident documentation  
- Tools-And-Skills.md — Tools, frameworks, and skills overview
