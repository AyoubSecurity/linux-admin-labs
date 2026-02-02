# Linux System Administration Labs

Hands-on Linux system administration labs designed to build **real-world Linux, security, and enterprise administration skills**, with a strong focus on **RHEL-based environments**.

Each lab is documented with:
- Clear objectives
- Step-by-step commands
- Configuration explanations
- Verification outputs
- Security and administration insights  
All reports are provided as **PDF overviews** written in LaTeX.

---

## Skills Covered

- Linux user and group management
- Filesystems, storage, and permissions
- Privilege escalation and sudo control
- Network configuration and services
- Firewall configuration and hardening
- SELinux concepts and enforcement
- System logging and auditing
- Security-oriented system administration

---

## Labs Completed

- **Lab A1 – Users & Groups**
  - User and group creation
  - UID/GID management
  - Account policies

- **Lab A2 – Disk Partitioning & Filesystems**
  - Partitioning with `fdisk`
  - Filesystem creation and mounting
  - Persistent mounts (`/etc/fstab`)

- **Lab A3 – Permissions & Ownership**
  - File and directory permissions
  - Ownership and group control
  - Special permissions (SUID, SGID, Sticky bit)

- **Lab A4 – sudo Privileges**
  - Sudoers configuration
  - Privilege delegation
  - Security implications of sudo access

- **Lab A5 – Network Configuration & Firewall Basics**
  - Network interface inspection
  - Service management with `systemctl`
  - Firewall configuration using `firewalld`
  - Securing SSH access

- **Lab A6 – SELinux Basics and Apache Context Management**
  - SELinux concepts and modes
  - Contexts, types, and labels
  - Troubleshooting access denials
  - Allowing Apache to serve content securely using SELinux

- **Lab A7 – System Logging and Auditing**
  - System logs and `journalctl`
  - Log persistence and filtering
  - Audit framework basics
  - Tracking security-relevant system events

---

## Repository Structure

linux-admin-labs/
├── LabA1/
├── LabA2/
├── LabA3/
├── LabA4/
├── LabA5/
├── LabA6/
├── LabA7/
└── README.md


Each lab directory contains:
- Compiled PDF overview
- Commands and results used during execution

---

## Goal

This repository documents a **progressive Linux administration learning path**, moving from fundamentals to **security-hardened, enterprise-ready system management**, suitable for:
- Linux system administrators
- Network engineers
- Cybersecurity engineers
- SOC / Blue Team preparation

---

## Next Labs (Planned)

- Lab A8 – Advanced firewalld and zones
- Lab A9 – User and service hardening
- Lab A10 – Cron, timers, and automation
- Lab A11 – Backup and recovery
- Lab A12 – System hardening checklist

---
