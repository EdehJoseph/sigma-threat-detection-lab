# PowerShell Encoded Command Detection

## Purpose
Detects PowerShell commands executed using Base64-encoded payloads.

## MITRE ATT&CK

- T1059.001 – PowerShell

## Severity

High

## Why attackers use it

Attackers often encode PowerShell commands to bypass security products, evade detection, and hide malicious scripts.

## Possible False Positives

- Legitimate administration scripts
- Automated deployment tools
- IT management software

## Recommended Response

- Identify the user who executed the command.
- Review the parent process.
- Decode the Base64 command.
- Check network connections initiated by PowerShell.
- Isolate the host if malicious activity is confirmed.

## Learning Outcome

Learned how Sigma detects suspicious PowerShell execution using encoded commands.