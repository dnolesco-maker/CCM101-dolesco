# Cloud Infrastructure Components

## 1. Compute Resources

### Purpose

Compute resources provide the processing power required to execute applications, perform calculations, and run operating systems. In cloud environments, compute resources can be provided through virtual machines, containers, or serverless services.

### Importance in Cloud Computing

Compute resources are important because they allow organizations to run applications and services without having to purchase and maintain physical servers. Cloud computing allows computing capacity to be provisioned and scaled according to workload requirements, providing flexibility and efficient resource utilization.

### KillerCoda Linux Environment

The KillerCoda Ubuntu 24.04.4 LTS environment provides a virtualized compute resource with an x86_64 architecture. Based on the `lscpu` command, the environment uses an Intel Xeon E312xx processor with 1 CPU and 1 CPU core. The system also reports KVM as the hypervisor with full virtualization, showing that the Linux environment is running as a virtualized cloud server.

| Compute Attribute | KillerCoda Finding |
|---|---|
| Architecture | x86_64 |
| CPU Model | Intel Xeon E312xx (Sandy Bridge, IBRS update) |
| CPU(s) | 1 |
| CPU Cores | 1 |
| Hypervisor | KVM |
| Virtualization | Full |

## 2. Storage Resources

### Purpose

Storage resources provide the space needed to store operating system files, applications, user data, and other information. In cloud computing, storage allows data to be stored and accessed by applications and users while providing flexibility for different storage requirements.

### Importance in Cloud Computing

Storage is important in cloud computing because applications and services need reliable space to store and retrieve data. Cloud storage also allows resources to be managed according to the needs of the workload without requiring organizations to maintain physical storage hardware themselves.

### KillerCoda Linux Environment

The KillerCoda Ubuntu 24.04.4 LTS environment uses a virtual disk named `vda` with a total size of 20 GB. The main root partition, `/dev/vda1`, provides 19 GB of storage and uses the ext4 filesystem. The environment also contains separate boot and EFI partitions used by the operating system.

| Storage Attribute | KillerCoda Finding |
|---|---|
| Virtual Disk | vda |
| Disk Size | 20 GB |
| Root Partition | /dev/vda1 |
| Root Partition Size | 19 GB |
| Root Filesystem | ext4 |
| Boot Partition | /dev/vda16 |
| Boot Filesystem | ext4 |
| EFI Partition | /dev/vda15 |
| EFI Filesystem | vfat |
