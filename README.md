# Linux System Administration & Security Labs (RHEL-Based)

Hands-on Linux system administration labs designed to build **enterprise-grade Linux, security, and automation skills** using a structured learning path based on **Red Hat Enterprise Linux (RHEL)**.

This repository documents a progressive journey from core administration fundamentals to **automation, system hardening, container security, and incident response readiness**.

All labs are written and documented in a professional format and provided as **PDF reports generated with LaTeX**.

---

## Learning Philosophy

This project follows a structured methodology:

- Real-world, enterprise-oriented configurations
- Security-first mindset
- Explicit command execution and validation
- Clear separation between control nodes and managed systems
- Infrastructure as code using Ansible
- Documentation suitable for professional portfolios

The goal is not only to learn Linux — but to build **resume-ready, production-oriented skills**.

---

## Skills Covered

### Core Linux Administration
- User and group management
- Filesystems and storage management
- Permissions and ownership control
- Privilege delegation using sudo
- Service management (`systemctl`)
- Network configuration and inspection

### Security & Hardening
- Firewall configuration with `firewalld`
- SSH access control
- SELinux modes, contexts, and policy troubleshooting
- Logging and auditing with `journalctl` and `auditd`
- Security-oriented configuration validation

### Automation & Infrastructure as Code
- Ansible control node setup
- SSH key-based automation
- Multi-host inventory configuration
- Privilege escalation with `become`
- Structured Ansible project layout
- Execution logging for traceability

---

## Labs Completed

### **Lab A1 – Users & Groups**
- User and group creation
- UID/GID concepts
- Account lifecycle basics

### **Lab A2 – Disk Partitioning & Filesystems**
- Disk identification
- Partitioning with `fdisk`
- Filesystem creation and mounting
- Persistent mounts with `/etc/fstab`

### **Lab A3 – Permissions & Ownership**
- File and directory permissions
- Ownership and group management
- Special permissions (SUID, SGID, Sticky bit)

### **Lab A4 – sudo Privileges**
- Sudoers configuration
- Least privilege delegation
- Security considerations for administrative access

### **Lab A5 – Networking & firewalld**
- Network interface inspection
- Service management
- Firewall configuration and rule management
- Securing SSH service

### **Lab A6 – SELinux Enforcement**
- SELinux modes (Enforcing, Permissive)
- Contexts and labels
- Troubleshooting access denials
- Secure Apache content serving under SELinux

### **Lab A7 – Logging & Auditing**
- `journalctl` usage and filtering
- Persistent logging
- Audit framework fundamentals
- Tracking security-relevant system activity

### **Lab A8 – Ansible Foundations**
- Ansible installation on control node
- SSH key-based authentication
- Multi-host inventory configuration
- Privilege escalation with sudo (`become`)
- Project-based Ansible configuration
- Logging and execution validation
- Managing:
  - `localhost`
  - Remote RHEL server (192.168.1.19)

---

## Repository Structure

linux-admin-labs/
├── Lab-A1/
├── Lab-A2/
├── Lab-A3/
├── Lab-A4/
├── Lab-A5/
├── Lab-A6/
├── Lab-A7/
├── Lab-A8/
│ ├── Lab_A8_Ansible_Foundations.pdf
│ ├── Lab_A8_Ansible_Foundations.tex
│ └── README.md
└── README.md


Each lab directory contains:
- Compiled LaTeX PDF report
- Structured command execution
- Validation results
- Enterprise-focused documentation

---

## Roadmap (Next Phases)

### Phase 1 – Ansible Automation (A9–A12)
- Ad-hoc commands and fact gathering
- Playbooks and idempotent configuration
- Roles and reusable automation structure
- Secure secret management with Ansible Vault

### Phase 2 – System Hardening & Visibility (A13–A15)
- SSH hardening and authentication control
- Kernel and sysctl security tuning
- Centralized logging concepts
- Baseline security enforcement

### Phase 3 – Reliability & Storage (A16–A18)
- LVM and snapshots
- Backup automation strategies
- Systemd advanced service control

### Phase 4 – Containers & Isolation (A19–A20)
- Podman containers on RHEL
- Rootless container security
- SELinux with containers
- Firewall isolation strategies

### Final Phase – Incident Awareness & Capstone
- Log triage and suspicious activity detection
- Service persistence investigation
- Infrastructure automation + hardening final project

---

## Long-Term Objective

This repository represents a structured path toward becoming:

- Enterprise Linux System Administrator
- Security-focused Infrastructure Engineer
- DevSecOps-ready Automation Engineer
- SOC / Blue Team oriented Linux specialist

The final objective is to demonstrate the ability to build:

- Automated
- Hardened
- Audited
- Documented
- Reproducible

Linux infrastructure in a production-oriented manner.

---

## Author

**Ayoub Zouargui**  
Master 1 – Networks and Embedded Systems  
University of Algiers 1  
Academic Year: 2025–2026  
GitHub: https://github.com/AyoubSecurity
