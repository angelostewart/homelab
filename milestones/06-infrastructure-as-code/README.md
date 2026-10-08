# 06 — Infrastructure as code

**Status:** Planned

## Goal

Codify the lab with Terraform and Ansible. Terraform gets a Proxmox module that clones the cloud-init template into N VMs, and an AWS module (VPC, EC2, and S3) with remote state in an S3 backend. Format, validate, and plan on every change. Ansible gets an inventory generated from Terraform outputs and roles for base hardening, users, and Node Exporter. Windows over WinRM is optional.

Machines: laptop, against Desktop 1 and AWS.

## Tasks

- [ ] Terraform: Proxmox module that clones the template into N VMs
- [ ] Terraform: AWS module for a VPC, EC2, and S3, with remote state in an S3 backend
- [ ] Run `fmt`, `validate`, and `plan` on every change
- [ ] Ansible: inventory generated from Terraform outputs
- [ ] Ansible roles for base hardening, users, and Node Exporter
- [ ] Optional: configure Windows over WinRM

## Skills

- Terraform
- Infrastructure as code
- Ansible
- Configuration management
- Python / YAML

## Target resume bullet

Codified hybrid infrastructure with Terraform (Proxmox + AWS, remote state) and Ansible roles; VMs go from zero to configured in minutes.

This is a target. It is not done yet.

## Notes

_None yet._

## Evidence

_None yet._
