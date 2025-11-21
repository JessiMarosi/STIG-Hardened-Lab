# Linux STIG Hardening Checklist

## User & Account Policies
- Disable root SSH login
- Enforce sudo access with audit trail
- Minimum password length: 14 characters, complexity enforced

## Services & Packages
- Disable unused services (cups, avahi, rpcbind)
- Ensure auditd installed and running
- Apply automatic security updates

## Firewall & Networking
- Configure iptables or ufw default deny
- Log all denied connections
- Restrict SSH to management network

## Evidence
- Screenshots of hardening checks
- Redacted configuration files
