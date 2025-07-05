# Ansible AWS EKS Node Bootstrap

This project uses Ansible to configure Amazon EKS worker nodes after they are provisioned with Terraform. It includes tools installation, SSH hardening, and CloudWatch logging setup.

## Features

- Install Docker and other essential packages
- Push CloudWatch logging configuration using Jinja2 template
- Harden SSH access with custom config
- Role-based structure for maintainability

## Usage

Ensure SSH access to EKS nodes and correct inventory IPs. Then run:

```bash
ansible-playbook playbooks/bootstrap.yml
