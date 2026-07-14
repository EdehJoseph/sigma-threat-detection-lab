# Mimikatz Detection

## Purpose

Detects activity associated with Mimikatz credential dumping.

## MITRE ATT&CK

- T1003 – OS Credential Dumping

## Severity

Critical

## Why attackers use it

Mimikatz extracts credentials from Windows memory, allowing attackers to move laterally and escalate privileges.

## Possible False Positives

- Security researchers
- Penetration testing
- Red team engagements

## Recommended Response

- Identify the affected endpoint.
- Check who launched Mimikatz.
- Reset compromised credentials.
- Investigate lateral movement.
- Review domain controller logs.

## Learning Outcome

Learned how Sigma rules detect credential dumping techniques used by attackers.