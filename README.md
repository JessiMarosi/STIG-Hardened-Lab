# STIG-Hardened-Lab

A reproducible, STIG-aligned Zero Trust lab environment demonstrating hardened endpoints, segmented networks, centralized identity, and evidentiary logging. Designed for cybersecurity practitioners, researchers, and recruiters to explore DoD-level best practices in a controlled lab setting.

---

## 🚀 Objectives

- Enforce **least privilege**, **microsegmentation**, and **continuous verification**
- Map configurations to **NIST 800-53** and relevant **STIG controls**
- Provide repeatable builds with automation and evidence artifacts
- Showcase practical skills in network hardening, endpoint security, and logging

---

## 🏗 Repository Structure

```
STIG-Hardened-Lab/
├── Docs/                  # Architecture, STIG checklists, hardening guides, reports
├── Configs/               # Configuration files for pfSense, Windows, Linux, network
├── Scripts/               # PowerShell, Bash, and Python automation scripts
├── Tools/                 # Scanners, analyzers, and automation tools
├── Evidence/              # Screenshots, logs, and sanitized configs (ignored)
├── Images/                # Lab images, diagrams
├── Diagrams/              # Network and architecture diagrams
├── VM-Files/              # VirtualBox/VM files (ignored)
└── README.md              # This file
```

> All sensitive files and evidence artifacts are ignored via `.gitignore`.

---

## ⚙️ Components

- **Perimeter:** pfSense firewall, VPN, VLAN segmentation  
- **Identity:** FreeIPA/OpenLDAP with MFA, RBAC, and audit logging  
- **Endpoints:** Windows + Ubuntu hardened to STIG benchmarks  
- **Telemetry:** Wazuh + ELK Stack for logging, monitoring, and alerts  
- **Automation:** Ansible roles + PowerShell helpers

---

## 📚 Usage

1. Clone this repository:

```bash
git clone https://github.com/JessiMarosi/STIG-Hardened-Lab.git
cd STIG-Hardened-Lab
```

2. Populate `Configs/`, `Scripts/`, and `VM-Files/` with your lab artifacts.  
3. Run automation scripts from `Scripts/` as required.  
4. Use `Docs/` for guidance, STIG checklists, and lab reports.  

---

## 🔒 Safety

- No secrets are stored in this repository  
- Use environment-specific vaults or placeholders for sensitive data  
- Evidence and VM files are ignored to prevent accidental exposure  

---

## 📌 Next Steps

- Build and harden VMs according to STIG checklists  
- Configure Zero Trust network segmentation  
- Integrate logging and telemetry into Wazuh + ELK  
- Automate common hardening tasks with PowerShell and Ansible
