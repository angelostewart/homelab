# homelab

Public notes for a home lab, kept while moving from systems administration into cloud and DevOps work. AWS is the main cloud. The on-prem side is two desktops and a laptop: a Proxmox host, a Windows Server domain controller, and an admin workstation.

The lab is just getting started. [Milestone 1](milestones/01-foundation/) (Proxmox on Desktop 1) is in progress. Milestones 2–10 are planned and not built. The dated log is in [PROGRESS.md](PROGRESS.md).

Maintained by [@angelostewart](https://github.com/angelostewart).

## Hardware

| Machine | Role | Notes |
| --- | --- | --- |
| Desktop 1 | Proxmox VE host | 32 GB DDR4, about 1 TB |
| Desktop 2 | Domain controller | Windows Server 2022 |
| Laptop | Admin and dev workstation | Where lab changes are written and applied |

Desktop 1 is the hypervisor and, later, the workload host. Desktop 2 is the on-prem identity anchor. The laptop is the day-to-day admin and development machine.

## Architecture

No diagram yet. The network and logical drawing will live in [`docs/diagrams/`](docs/diagrams/) once the IP layout and VLANs are planned in milestone 1. That folder will hold the source file and an exported image.

## Milestones

| # | Milestone | Status |
| --- | --- | --- |
| 1 | [Foundation](milestones/01-foundation/) | In progress |
| 2 | [AD core](milestones/02-ad-core/) | Planned |
| 3 | [Dev workstation, Linux, and Git](milestones/03-dev-workstation/) | Planned |
| 4 | [Hybrid identity](milestones/04-hybrid-identity/) | Planned |
| 5 | [Cloud foundations](milestones/05-cloud-foundations/) | Planned |
| 6 | [Infrastructure as code](milestones/06-infrastructure-as-code/) | Planned |
| 7 | [Containers](milestones/07-containers/) | Planned |
| 8 | [Kubernetes](milestones/08-kubernetes/) | Planned |
| 9 | [CI/CD](milestones/09-cicd/) | Planned |
| 10 | [Observability and DR](milestones/10-observability-dr/) | Planned |

## Skills

Each mark is a skill that milestone is planned to show. Nothing in this table is finished work.

| Skill | 01 | 02 | 03 | 04 | 05 | 06 | 07 | 08 | 09 | 10 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Virtualization | ✓ |  |  |  |  |  |  |  |  |  |
| Linux | ✓ |  | ✓ |  |  |  |  | ✓ |  |  |
| Networking basics | ✓ |  |  |  |  |  |  |  |  |  |
| Documentation | ✓ |  |  |  |  |  |  |  |  |  |
| Active Directory |  | ✓ |  |  |  |  |  |  |  |  |
| DNS / DHCP |  | ✓ |  |  |  |  |  |  |  |  |
| PowerShell |  | ✓ |  |  |  |  |  |  |  |  |
| Bash |  |  | ✓ |  |  |  |  |  |  |  |
| Git |  |  | ✓ |  |  |  |  |  |  |  |
| SSH |  |  | ✓ |  |  |  |  |  |  |  |
| Security hardening |  |  | ✓ |  |  |  |  |  |  |  |
| Entra ID |  |  |  | ✓ |  |  |  |  |  |  |
| IAM |  |  |  | ✓ | ✓ |  |  |  |  |  |
| Hybrid identity |  |  |  | ✓ |  |  |  |  |  |  |
| MFA |  |  |  | ✓ |  |  |  |  |  |  |
| AWS |  |  |  |  | ✓ |  |  |  |  |  |
| Cloud networking |  |  |  |  | ✓ |  |  |  |  |  |
| Cost management |  |  |  |  | ✓ |  |  |  |  |  |
| Terraform |  |  |  |  |  | ✓ |  |  |  |  |
| Infrastructure as code |  |  |  |  |  | ✓ |  |  |  |  |
| Ansible |  |  |  |  |  | ✓ |  |  |  |  |
| Configuration management |  |  |  |  |  | ✓ |  |  |  |  |
| Python |  |  |  |  |  | ✓ | ✓ |  |  |  |
| YAML |  |  |  |  |  | ✓ |  |  |  |  |
| Docker |  |  |  |  |  |  | ✓ |  |  |  |
| Container security |  |  |  |  |  |  | ✓ |  |  |  |
| Kubernetes |  |  |  |  |  |  |  | ✓ |  |  |
| Helm |  |  |  |  |  |  |  | ✓ |  |  |
| Troubleshooting |  |  |  |  |  |  |  | ✓ |  |  |
| CI/CD |  |  |  |  |  |  |  |  | ✓ |  |
| GitHub Actions |  |  |  |  |  |  |  |  | ✓ |  |
| GitOps |  |  |  |  |  |  |  |  | ✓ |  |
| Secrets management |  |  |  |  |  |  |  |  | ✓ |  |
| DevSecOps |  |  |  |  |  |  |  |  | ✓ |  |
| Monitoring (Prometheus / Grafana) |  |  |  |  |  |  |  |  |  | ✓ |
| Logging |  |  |  |  |  |  |  |  |  | ✓ |
| Alerting |  |  |  |  |  |  |  |  |  | ✓ |
| Backup / DR |  |  |  |  |  |  |  |  |  | ✓ |
| SRE mindset |  |  |  |  |  |  |  |  |  | ✓ |

Column numbers match the milestone table. A mark means that milestone is where the skill is practiced.

## Repository layout

Placeholder folders only. Code lands in a folder when that milestone starts.

| Path | Purpose |
| --- | --- |
| [`docs/diagrams/`](docs/diagrams/) | Network and logical diagrams |
| [`docs/runbooks/`](docs/runbooks/) | Rebuild and recovery steps |
| [`docs/adr/`](docs/adr/) | Architecture decision records |
| [`docs/incidents/`](docs/incidents/) | Break-fix write-ups |
| [`terraform/`](terraform/) | Proxmox and AWS Terraform |
| [`ansible/`](ansible/) | Inventories and roles |
| [`k8s/`](k8s/) | Manifests and Helm |
| [`app/`](app/) | Containerized lab app |
| [`scripts/`](scripts/) | PowerShell and Bash |
| [`milestones/`](milestones/) | One folder per milestone |

## No secrets in this repo

This repository is public. Do not commit passwords, tokens, cloud credentials, SSH private keys, kubeconfigs, Terraform state, `*.tfvars`, `.env` files, or Ansible vault password files. `.gitignore` is set up for those. Use a password manager, GitHub Actions secrets or OIDC, and Ansible Vault when a later milestone needs a secret. If a secret is committed, rotate it.
