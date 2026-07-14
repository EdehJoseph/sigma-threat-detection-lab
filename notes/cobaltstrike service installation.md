# Cobalt Strike Service Installation Detection

## Purpose

Detects malicious Windows services installed by Cobalt Strike during privilege escalation or lateral movement.

## MITRE ATT&CK

- T1021.002 – SMB/Windows Admin Shares
- T1543.003 – Windows Service
- T1569.002 – Service Execution

## Severity

High

## Why attackers use it

Cobalt Strike commonly installs malicious services to maintain persistence and execute payloads with elevated privileges.

## Possible False Positives

- Authorized penetration testing
- Red team exercises

## Recommended Response

- Review the service executable path.
- Verify whether the service is legitimate.
- Check the parent process.
- Investigate PowerShell usage.
- Remove malicious services and isolate the endpoint.

## Learning Outcome

Learned how Sigma detects Cobalt Strike persistence and service creation techniques.