# Enterprise Cloud Architec

## 1. System Overview & Architecture
* **Virtualization:** Oracle VM VirtualBox running Ubuntu Server 64-bit with the network adapter set to Bridged Adapter mode.
* **Networking:** Fixed Static IP configuration (`192.168.1.58/24`) managed via Netplan (`/etc/netplan/00-installer-config.yaml`).
* **Containerization:** Docker & Docker Compose orchestrating an enterprise WordPress web application tied to an isolated MySQL database container (`enterprise_mysql_db`) with persistent storage volumes.
* **Automation:** Shell script automation for dynamic database backups, compression, and maintenance logs.

---

## 2. Directory Structure
```text
CCM101-dolesco/
└── Laboratory-10-Enterprise-Cloud-Architec/
    ├── .env
    ├── README.md
    ├── architecture-diagram.png
    ├── automation-script.sh
    ├── backup-wordpress.sh
    ├── docker-compose.yml
    ├── final-reflection.md
    └── operational-manual.md
