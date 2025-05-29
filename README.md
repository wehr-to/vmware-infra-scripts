# 🖥️ vmware-infra-scripts

A curated collection of scripts for automating and managing VMware vSphere infrastructure — including PowerCLI, PyVmomi (Python SDK), and Bash guest OS operations.

This repo is designed for platform engineers, sysadmins, and DevOps professionals working in hybrid and on-prem VMware environments.

## 📌 Purpose

This repository provides practical automation tools to:

- Manage VMs and templates across vCenter
- Run compliance and inventory audits
- Enforce hardening policies
- Automate day-to-day vSphere tasks

All scripts are written to be modular, easily testable, and cross-functional across enterprise environments.

## 🧱 Folder Breakdown

| Folder                | Description                                                      |
|------------------------|------------------------------------------------------------------|
| `powercli-scripts/`     | PowerShell scripts using PowerCLI modules                      |
| `pyvmomi-scripts/`      | Python automation using VMware's vSphere Python SDK            |
| `bash-vm-guest/`        | Bash scripts executed inside Linux guest VMs                   |
| `security-hardening/`   | Scripts and docs for host hardening and compliance             |
| `docs/`                 | Reference guides, snapshot strategies, and tool checks         |
| `examples/`             | Sample output and screenshots from script runs                 |

## 🔧 PowerCLI Scripts

- `snapshot-management.ps1`: Report and delete old snapshots
- `vm-health-report.ps1`: Pull CPU, memory, and disk stats across all VMs
- `deploy-vm-template.ps1`: Deploy a VM from template with custom specs

## 🐍 PyVmomi Scripts

- `list-vms.py`: Lists all VMs across datacenters
- `connect-to-vcenter.py`: Boilerplate for vCenter API access
- `tag-compliance-check.py`: Audit VM tags for backup/compliance status

## 🛡️ Security Hardening

- Disable unnecessary services (SSH, Shell, ESXi Shell)
- Audit VM snapshots and untagged machines
- Checklist for VM Tools health and patch visibility

## 🧠 Use Cases

- Cert Prep (VCP-DCV, VM Admin)
- Internal lab setup
- Audit scripting for asset inventory
- Resume/showcase for automation skills

## ⚙️ Requirements

- PowerCLI 13.x+
- Python 3.10+ + `pyvmomi`
- Access to vCenter or ESXi lab
- VMware Tools installed on guest VMs

## 🚀 Roadmap

- [ ] Add automated patch baseline evaluator
- [ ] Add VM lifecycle automation (create → power on → tag → delete)
- [ ] Create unified audit report across PowerCLI + PyVmomi
- [ ] Add YAML-based input for bulk VM deployments

## 🤝 Contributions

Pull requests are welcome — especially new scripts, integrations, or hardening documentation. Please submit clean, modular code with inline comments.


