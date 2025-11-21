# pfSense STIG Hardening Checklist

## Interfaces
- WAN: NAT or external network
- LAN: Internal lab segment
- DMZ: Optional

## Admin Access
- Change default admin username
- Enforce MFA for web GUI and SSH
- Restrict admin access to management VLAN

## Firewall Rules
- Default deny all inbound/outbound except required services
- Log all rule hits
- Use aliases for IPs/networks for easier management

## Services
- Disable UPnP, Captive Portal, unused services
- Enable NTP from trusted sources
- Enable remote syslog to Wazuh/ELK

## Evidence
- Screenshots of VLANs, rules, logs
- Redacted configuration exports
