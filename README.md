# Ansible Learning Lab

Welcome to my **Ansible Learning Lab**! 🎓  
This repository serves as a hands-on workspace to explore, practice, and master [Ansible](https://www.ansible.com/) — the powerful, agentless automation tool for configuration management, application deployment, orchestration, and more.

---

## 🎯 Objectives

- Learn Ansible core concepts (playbooks, roles, inventories, modules, variables, etc.)
- Practice writing clean, reusable, and idempotent automation
- Automate infrastructure provisioning and configuration
- Integrate Ansible with real-world tools like Vagrant, Docker, and cloud platforms
- Prepare for real-world DevOps and system engineering tasks

---

## 📁 Repository Structure

```
ansible-learning-lab/
├── README.md
├── inventory/   # Inventory files (static & dynamic)
├── playbooks/   # Example playbooks for various use cases
├── roles/       # Custom and reusable Ansible roles
├── group_vars/  # Group-level variables
├── host_vars/   # Host-specific variables
├── templates/   # Jinja2 templates for config files
├── files/       # Static files to be copied to hosts
├── experiments/ # Sandbox area for testing new concepts
└── docs/        # Notes, diagrams, and learning references
```

---

## 🚀 Getting Started

### Prerequisites

- Linux (preferably Linux Mint or RHEL-based)
- Python 3.8+
- `pip` package manager
- SSH access to target machines (or local virtual machines via Vagrant)

### Install Ansible

```bash
# Enable the official Red Hat Ansible Automation Platform 2.6 repository for RHEL 9 (x86_64 architecture)
sudo subscription-manager repos --enable ansible-automation-platform-2.6-for-rhel-9-x86_64-rpms

# Update all installed packages to their latest versions to ensure system stability and security
sudo dnf update -y

# Install the core Ansible execution engine (`ansible-core`) and the CLI-based automation navigator (`ansible-navigator`)
sudo dnf install -y ansible-core ansible-navigator
```

## 🧪 Recommended Learning Path

1. Basics: Inventory, ad-hoc commands, simple playbooks
2. Variables & Templating: group_vars, host_vars, templates/
3. Roles: Structure reusable automation units
4. Handlers & Conditions: Control task execution flow
5. Loops & Blocks: Write efficient and dynamic tasks
6. Vault: Securely manage secrets (ansible-vault)
7. Testing: Use molecule or manual VMs for role validation
8. Integration: Combine with Vagrant, Packer, or cloud providers (AWS/Azure)

## 🛠 Tools in My Stack (Context)

- **Hypervisor:** VMware Workstation
- **Guest OS:** Red Hat Enterprise Linux (RHEL)
- **Local Dev:** Linux Mint
- **CI/CD:88 GitLab (future integration planned)
- **Monitoring:** Prometheus + Grafana + Loki (for observability of automated systems)

