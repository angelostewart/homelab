# 09 — CI/CD

**Status:** Planned

## Goal

Add GitHub Actions for this repo. On a pull request: lint, test, build, Trivy scan, and `terraform plan`. On merge: push the image and deploy to k3s through a self-hosted runner VM on Proxmox. Authenticate to AWS with OIDC so the workflow has no long-lived keys, and require approval before `terraform apply`. Argo CD for GitOps is optional.

Machines: Desktop 1 (runner), GitHub, and AWS.

## Tasks

- [ ] GitHub Actions on pull request: lint, test, build, Trivy scan, and `terraform plan`
- [ ] On merge: push the image and deploy to k3s through a self-hosted runner VM on Proxmox
- [ ] Authenticate to AWS with OIDC (no long-lived keys)
- [ ] Gate `terraform apply` on approval
- [ ] Optional: Argo CD for GitOps

## Skills

- CI/CD
- GitHub Actions
- GitOps
- Secrets management
- DevSecOps

## Target resume bullet

Built CI/CD pipelines in GitHub Actions (test, scan, build, Terraform plan/apply, deploy to Kubernetes) using OIDC and a self-hosted runner.

This is a target. It is not done yet.

## Notes

_None yet._

## Evidence

_None yet._
