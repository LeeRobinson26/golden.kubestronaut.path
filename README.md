# golden.kubestronaut.path
Golden Kubestronaut Journey: Notes, Failures, and Successes

# 🎖️ Golden Kubestronaut Journey

> **Candidate:** Lee Robinson  
> **Target Achievement:** CNCF Golden Kubestronaut  
> **Deadline:** Q4 2026  
> **Lab Environment:** Dell PowerEdge R730 (Hybrid Cloud) & VMware Workstation

---

## 🚀 The Mission
To achieve "Golden" status by mastering the full CNCF landscape—from foundational Linux administration (LFCS) to advanced platform engineering (Backstage/Crossplane). This repository serves as the **Source of Truth** for my automated lab environments, study notes, and architectural patterns.

## 📊 Certification Roadmap

| Status | Certification | Target Date | Exam Code |
| :---: | :--- | :---: | :--- |
| 🔄 | **LFCS** (Linux Foundation Certified SysAdmin) | Q1 2026 | Recertification |
| 🔄 | **CKA** (Certified Kubernetes Administrator) | Q1 2026 | Recertification |
| 📅 | **CKAD** (Certified Kubernetes Application Developer) | Q1 2026 | Recertification |
| 📅 | **CKS** (Certified Kubernetes Security Specialist) | Q2 2026 | New |
| ✅ | **KCNA/KCSA** (Cloud Native & Security Assoc.) | Q1 | — |
| 🏗️ | **Golden Tier** (PCA, ICA, CCA, CAPA, etc.) | Ongoing | Multi-cert |

*Key: ✅ Completed | 🔄 In Progress | 📅 Scheduled | 🔒 Prerequisite Locked*

---

## 🏗️ Architectural "Golden Path"
This repo implements a "Bottom-Up" architecture. Each folder in `/infra` and `/automation` follows this lifecycle:

1. **Bootstrap:** Packer + Ansible (Immutable Images)
2. **Provision:** Terraform (R730/Workstation Resources)
3. **Platform:** Crossplane (Cloud-Native Infrastructure Management)
4. **Security/Networking:** Cilium + Istio + Kyverno (The Guardrails)
5. **Observation:** OpenTelemetry + Prometheus + Jaeger
6. **GitOps:** ArgoCD + Kustomize/Helm (Continuous Delivery)
7. **Portal:** Backstage (The Developer Interface)

---

## 📂 Repository Structure

- `📂 exams/`: Domain-specific checklists and "Chaos Engineering" scripts to break/fix objectives.
- `📂 infra/`: Terraform and VMware Workstation `.vmx` automation.
- `📂 automation/`: Ansible playbooks for Day 0 hardening and Crossplane Compositions.
- `📂 manifests/`: Kustomize overlays and Helm charts for the Golden Path tools.
- `📂 scripts/`: Lab-reset tools using `vmrun` and `kubectl` power-user aliases.

---

## 🛠️ Lab Setup (A-Z)
### Quick-Win Layer (Laptop)
- **Host:** VMware Workstation
- **Automation:** Vagrant + `vmrun`
- **Focus:** LFCS CLI tasks, CKA Troubleshooting, KCNA/KCSA theory.

### Production Layer (R730)
- **Host:** Dell PowerEdge R730 (ESXi/Proxmox)
- **Automation:** Terraform + Ansible
- **Focus:** Multi-node HA Clusters, CKS Security auditing, Crossplane-managed AWS/GCP resources.

---

## 🔗 Quick Links
- [CNCF Kubestronaut Program](https://www.cncf.io/kubestronaut/)
- [Official Exam Documentation (Allowed during tests)](docs/bookmarks.md)
- [My Study Schedule](docs/schedule.md)

---
*"The only way to be sure of your architecture is to try and break it every day."*
