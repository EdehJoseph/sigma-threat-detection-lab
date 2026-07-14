# Failed Logon Detection

## Purpose

Detects repeated failed login attempts that may indicate password attacks.

## MITRE ATT&CK

- T1110 – Brute Force

## Severity

Medium

## Why attackers use it

Attackers repeatedly attempt different passwords until they successfully authenticate.

## Possible False Positives

- Users forgetting passwords
- Expired credentials
- Service account failures

## Recommended Response

- Review failed login source IPs.
- Determine whether multiple accounts are targeted.
- Lock compromised accounts if necessary.
- Enable MFA.
- Block malicious IP addresses.

## Learning Outcome

Learned how authentication logs help detect brute-force attacks.