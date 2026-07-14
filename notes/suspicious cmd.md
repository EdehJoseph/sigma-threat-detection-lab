# Suspicious Command Execution

## Purpose

Detects execution of suspicious Windows command-line activity.

## MITRE ATT&CK

- T1059 – Command and Scripting Interpreter

## Severity

Medium

## Why attackers use it

Attackers abuse command-line tools to download malware, enumerate systems, create users, or disable security software.

## Possible False Positives

- System administrators
- Automation scripts
- Enterprise management tools

## Recommended Response

- Review the executed command.
- Identify the parent process.
- Check user privileges.
- Review subsequent activity.
- Investigate downloaded files.

## Learning Outcome

Learned how Sigma identifies suspicious command-line behavior.