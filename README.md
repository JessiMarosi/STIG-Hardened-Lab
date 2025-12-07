# STIG-Hardened-Lab

A reproducible, STIG-aligned Zero Trust lab environment demonstrating hardened endpoints, segmented networks, centralized identity, and evidentiary logging. Designed for cybersecurity practitioners, researchers, and recruiters to explore DoD-level best practices in a controlled lab setting.

---

## 🚀 Objectives

- Enforce **least privilege**, **microsegmentation**, and **continuous verification**  
- Map configurations to **NIST 800-53** and relevant **STIG controls**  
- Provide repeatable builds with automation and evidence artifacts  
- Showcase practical skills in network hardening, endpoint security, and logging  

---

## 📊 Impact & Results

- Reduced High/Critical vulnerabilities by **78%** across pfSense firewall and OpenVPN stack, validated by Nessus scans  
- Progressed Lynis hardening index from **63 → 77** through kernel tuning, persistent auditd, and AIDE validation  
- Implemented **>40 STIG-aligned controls** with reproducible documentation and 25+ audit artifacts  
- Enforced Zero Trust segmentation with **12 firewall rules across 4 zones**, ensuring compliance and forensic credibility  

---

## 🏗 Repository Structure

```plaintext
STIG-Hardened-Lab/
├── Configs/           # Hardened system configs, STIG checklists, and remediation templates
├── Diagrams/          # Architecture diagrams, flowcharts, and lab topology visuals
├── Docs/              # STIG documentation, SOPs, and audit-grade writeups
├── Evidence/          # Screenshots, logs, and forensic proof of hardening steps
├── Images/            # Visual assets used in documentation and dashboards
├── Scripts/           # PowerShell, Bash, and Python automation for STIG enforcement
├── Tools/             # Utilities and helper binaries used during hardening
├── VM-Files/          # Virtual machine exports, snapshots, and configuration files
├── .gitignore         # Excludes sensitive and platform-specific clutter
├── LICENSE            # MIT license for public use and adaptation
└── README.md          # Project overview, usage instructions, and recruiter-facing notes
