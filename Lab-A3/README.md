# Lab A3 — User, Group, and Permission Management (RHEL)

## Objective
This lab focuses on identity and access management on Red Hat Enterprise Linux. The goal is to create users and groups, manage permissions, and enforce controlled access to shared system resources.

## Environment
- OS: Red Hat Enterprise Linux
- Machine: Single RHEL admin workstation
- Privileges: sudo-enabled administrative user

## Tasks Performed
- Created administrative and application groups
- Created user accounts and assigned group memberships
- Set and managed user passwords
- Reviewed Linux account databases
- Configured directory ownership and permissions
- Validated access restrictions

## Key Commands Used
- `useradd`, `groupadd`, `usermod`
- `passwd`
- `id`
- `chmod`, `chown`
- `su`, `sudo`

## Security Notes
Administrative users do not bypass filesystem permissions. Access must be explicitly granted via group membership, ACLs, or root privileges. This behavior enforces the principle of least privilege.

## Outcome
The system correctly restricted access to shared resources based on permissions, demonstrating proper Linux access control behavior.

## Next Lab
Lab A4 will focus on privilege delegation using `sudo`, secure administrative access, and system hardening basics.
