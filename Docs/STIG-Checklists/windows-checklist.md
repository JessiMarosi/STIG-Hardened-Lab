# Windows STIG Hardening Checklist

## Account Policies
- Minimum password length: 14 characters
- Enforce complexity and expiration
- Lockout threshold: 5 failed attempts

## Services
- Disable unnecessary services (SMBv1, Remote Registry)
- Enable Windows Defender with automatic updates

## Auditing & Logging
- Enable audit for logon events, object access, and policy changes
- Forward logs to central Wazuh/ELK server

## Evidence
- Screenshots of Group Policy settings
- Redacted exported registry keys or security baseline reports
