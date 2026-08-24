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
