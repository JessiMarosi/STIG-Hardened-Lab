# STIG-Hardened-Lab

A reproducible, STIG-aligned Zero Trust reference lab that demonstrates hardened endpoints, segmented networks, centralized identity, and evidentiary logging. This repository is designed to be reviewable: configurations, procedures, and validation artifacts are organized to support audit-style scrutiny.

## What This Demonstrates

This lab is built to show operational security work in a form that government and critical-infrastructure reviewers recognize:

- STIG-aligned hardening implemented as repeatable configuration and scripted enforcement
- Network segmentation consistent with Zero Trust principles (explicit zones and rule justification)
- Validation using standard security assessment tooling with retained evidence artifacts
- Audit-style documentation linking controls → implementation → verification → evidence

## Architecture Summary

The lab implements segmented zones with explicit allow/deny policy and centralized visibility.

- Perimeter and segmentation: firewall routing and zone policy
- Remote access: VPN configuration with hardened defaults
- Endpoints: host-level hardening and logging
- Evidence: retained scans, logs, and screenshots supporting each major control set

See `Diagrams/` for topology and flow documentation.

## Results (Representative)

The repository includes validation artifacts demonstrating measurable hardening outcomes, such as:

- Reduced High/Critical findings on perimeter/VPN components based on vulnerability scan outputs
- Improved host hardening posture based on configuration and integrity monitoring validation
- Implemented STIG-aligned controls with corresponding evidence artifacts

See `Evidence/` and `Docs/` for raw outputs and writeups.

## Repository Structure

- `Configs/` — Hardened configuration files, templates, and remediation references
- `Scripts/` — Automation for enforcement and repeatability (PowerShell/Bash/Python)
- `Docs/` — SOPs, control notes, and audit-grade writeups
- `Evidence/` — Screenshots, logs, and scan outputs supporting claims
- `Diagrams/` — Topology and workflow visuals
- `Tools/` — Helper utilities used during build/hardening (no sensitive binaries committed)
- `VM-Files/` — Non-sensitive VM configuration references only (no exported images)

## Reproduce the Lab

This repository is organized around a repeatable workflow:

1. Build the lab environment
2. Apply hardening baselines
3. Validate posture with scans and system checks
4. Capture evidence artifacts in a consistent structure
5. Review control-to-evidence traceability

Start with:
- `Docs/BUILD_SOP.md`
- `Docs/HARDENING_SOP.md`
- `Docs/VALIDATION_SOP.md`
- `Docs/EVIDENCE_SOP.md`

## Control-to-Evidence Traceability

The lab is intended to be auditable. Control implementation and verification evidence are indexed here:

- `Docs/CONTROL_CATALOG.md` — implemented controls and status
- `Docs/MAPPING_NIST_800_53.md` — mapping for implemented controls (selected)

## Security and Privacy

This repository intentionally excludes:
- credentials, tokens, private keys, and secrets
- exported VM images or snapshots
- logs containing personal or sensitive identifiers

If you discover sensitive content, open an issue with a minimal description and no secrets.

## License

MIT License. See `LICENSE`.
