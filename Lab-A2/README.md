# Lab A2 — RHEL Storage Management (Partitions and Filesystems)

## Objective
This lab introduces fundamental storage administration on Red Hat Enterprise Linux. The objective is to identify existing disks, create a new partition, format it with a Linux filesystem, mount it, and configure persistent mounting. These skills are essential for Linux system administration, server management, and enterprise environments.

## Lab Environment
- Operating System: Red Hat Enterprise Linux
- Machine: Single RHEL Admin Workstation (Virtual Machine)
- Disk Layout:
  - /dev/sda — 15 GB system disk
  - /dev/sr0 — ISO device (read-only, not used)
- Note: No separate server node is required for this lab.

## Procedure

### 1. Identify Available Block Devices
```bash
lsblk
```
Displays all detected block devices and their partition layout. Only `/dev/sda` is used in this lab.

### 2. Create a New Partition
```bash
sudo fdisk /dev/sda
```
Inside the `fdisk` interactive prompt, enter the following exactly:
```
n
p
3
<Enter>
<Enter>
w
```
Explanation:
- `n` creates a new partition
- `p` selects a primary partition
- `3` chooses the partition number
- Pressing Enter twice accepts default start and end sectors
- `w` writes the partition table to disk

### 3. Create a Filesystem
```bash
sudo mkfs.ext4 /dev/sda3
```
Formats the new partition using the EXT4 filesystem.

### 4. Create a Mount Point
```bash
sudo mkdir /data
```
Creates the directory that will host the filesystem.

### 5. Mount the Filesystem
```bash
sudo mount /dev/sda3 /data
```
Verify the mount:
```bash
df -h
```

### 6. Configure Persistent Mounting
Retrieve the partition UUID:
```bash
sudo blkid /dev/sda3
```
Edit the filesystem table:
```bash
sudo nano /etc/fstab
```
Add the following line (replace `<UUID_HERE>` with the actual UUID):
```
UUID=<UUID_HERE>  /data  ext4  defaults  0  0
```
Test the configuration:
```bash
sudo mount -a
```
No output indicates the configuration is correct.

## Command Notes (Quick Reference)
- `lsblk` — List disks and partitions
- `fdisk` — Create and manage disk partitions
- `mkfs.ext4` — Create an EXT4 filesystem
- `mount` — Attach a filesystem to a directory
- `blkid` — Display partition UUIDs
- `/etc/fstab` — Configure automatic mounting at boot

## Validation
- `/dev/sda3` appears in `lsblk`
- Filesystem type is `ext4`
- Mounted at `/data`
- Mount persists after reboot

## Skills Acquired
- Disk and partition management
- Filesystem creation and mounting
- Persistent storage configuration
- Core Red Hat Enterprise Linux administration skills
