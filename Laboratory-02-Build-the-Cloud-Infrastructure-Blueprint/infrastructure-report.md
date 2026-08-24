# Infrastructure Report

## Checkpoint 2 – Investigate the Cloud Server

This report documents the system information collected from the KillerCoda Ubuntu 24.04 environment.

## 1. Operating System

- **Operating System:** Ubuntu 24.04.4 LTS
- **Version ID:** 24.04
- **Codename:** Noble Numbat

The cloud server is running Ubuntu 24.04.4 LTS, a Linux-based operating system.

## 2. Kernel

- **Kernel Version:** 6.8.0-138-generic

The kernel is the core component of the Linux operating system that manages system resources and communication between hardware and software.

## 3. CPU / Compute

- **CPU Architecture:** x86_64
- **CPU Model:** Intel Xeon E312xx (Sandy Bridge, IBRS update)
- **CPU(s):** 1
- **CPU Cores:** 1
- **Hypervisor:** KVM
- **Virtualization Type:** Full

The environment provides one virtual CPU core. The `lscpu` output also identifies KVM as the hypervisor and full virtualization as the virtualization type.

## 4. Memory

- **Total RAM:** 1.9 GiB
- **Used:** 412 MiB
- **Free:** 840 MiB
- **Available:** 1.5 GiB
- **Swap:** 1.0 GiB

The server has approximately 1.9 GiB of allocated RAM.

## 5. Storage

- **Virtual Disk:** 20 GB
- **Root Partition:** 19 GB
- **Root File System:** ext4

The system uses a 20 GB virtual disk named `vda`. The main root partition is approximately 19 GB.

## 6. Mounted File Systems

| Device | File System | Size | Mounted On |
|---|---|---:|---|
| `/dev/vda1` | ext4 | 19G | `/` |
| `/dev/vda16` | ext4 | 881M | `/boot` |
| `/dev/vda15` | vfat | 105M | `/boot/efi` |

Additional temporary file systems such as `tmpfs` are mounted at `/run`, `/dev/shm`, and `/run/lock`.

## 7. Hostname

- **Hostname:** ubuntu

The hostname assigned to the cloud server is `ubuntu`.

## 8. IP Address

The server returned the following IP addresses:

- `172.30.1.2`
- `172.17.0.1`

These addresses were obtained using the `hostname -I` command.

## 9. System Summary

| Category | Finding |
|---|---|
| Operating System | Ubuntu 24.04.4 LTS |
| Kernel | 6.8.0-138-generic |
| CPU | Intel Xeon E312xx (Sandy Bridge, IBRS update) |
| CPU Cores | 1 |
| RAM | 1.9 GiB |
| Virtual Disk | 20 GB |
| Root Partition | 19 GB |
| Root File System | ext4 |
| Hostname | ubuntu |
| IP Addresses | 172.30.1.2, 172.17.0.1 |
| Hypervisor | KVM |
| Virtualization | Full |

## Evidence

The server investigation evidence is saved in:

`/screenshots/server-investigation.png`
