# Proxmox DevOps & Cybersecurity Lab

## Overview
This repository documents a private cloud lab environment built on **Proxmox VE**, showcasing **DevOps automation** and **Cybersecurity monitoring**.  
It demonstrates enterprise‑style infrastructure using **IaC (Terraform + Ansible)**, **K3s HA clusters**, **Wazuh SIEM**, **GitLab CI/CD**, and **Prometheus/Grafana** monitoring.

The project is designed as my portfolio artifact, proving hands‑on capability in virtualization, orchestration, automation, and security.



##  Environment & Resource Plan
- **Host:** Laptop/PC (24GB RAM, 4‑Core CPU, 512GB SSD)
- **RAM Allocation:**
  - OPNsense Firewall: 1GB  
  - NFS Storage (Debian LXC): 512MB  
  - K3s Cluster (3 Nodes): 12GB (4GB each)  
  - Wazuh SIEM Manager: 4GB  
  - GitLab CI/CD: 6GB  
  - Proxmox Overhead: 4GB  
  - Buffer: 2GB  



## Modules
- **Module 1:** Network & Hypervisor Foundation (Proxmox + OPNsense)  
- **Module 2:** Shared Services & Storage (NFS LXC)  
- **Module 3:** Infrastructure as Code (Terraform + Proxmox API)  
- **Module 4:** Orchestration (K3s Cluster via Ansible)  
- **Module 6:** High Availability & SIEM (PostgreSQL DB + Wazuh Manager)  
- **Module 7:** CI/CD Pipeline (GitLab + Runners)  
- **Module 8:** Monitoring (Prometheus + Grafana)  



## Validation Checklist
| Component   | Validation Command / Action |
|-------------|-----------------------------|
| OPNsense    | `ping 10.10.10.1` |
| NFS LXC     | `showmount -e 10.10.40.10` |
| K3s Cluster | `kubectl get nodes` |
| Wazuh SIEM  | Agents visible in dashboard |
| GitLab CI/CD| Pipeline runs on commit |
| Monitoring  | Grafana dashboards show metrics |



## Technical Skills
This lab demonstrates:
- **Virtualization & Networking** (Proxmox, VLANs, OPNsense)  
- **Automation** (Terraform, Ansible, GitLab CI/CD)  
- **Resilience** (K3s HA cluster with external DB)  
- **Security** (Wazuh SIEM integration)  
- **Observability** (Prometheus + Grafana monitoring)  

## Roles
- DevOps
- Cybersecurity
- SOC Analyst
- Pen Tester
- Security Engineer



## 📜 License
This project is licensed under the **MIT License**.  
You are free to use, modify, and share with attribution.