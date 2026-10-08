# 10 — Observability and DR

**Status:** Planned

## Goal

Install kube-prometheus-stack (Prometheus, Grafana, Alertmanager) and Loki. Dashboard k3s, Linux hosts, the Windows domain controller (windows_exporter), and the app. Send alerts to Discord or email. Back up Proxmox, snapshot etcd/k3s, and copy backups to S3. Capstone: wipe the k3s VMs, rebuild them from this repo, time the recovery, and write it up.

Machines: Desktop 1, Desktop 2, and AWS.

## Tasks

- [ ] Install kube-prometheus-stack (Prometheus, Grafana, Alertmanager) and Loki
- [ ] Build dashboards for k3s, Linux, the Windows DC (windows_exporter), and the app
- [ ] Send alerts to Discord or email
- [ ] Set up Proxmox backups
- [ ] Set up etcd/k3s snapshots and S3 copies offsite
- [ ] Capstone: wipe the k3s VMs, rebuild them from this repo, time the recovery, and write it up

## Skills

- Monitoring (Prometheus / Grafana)
- Logging
- Alerting
- Backup / DR
- SRE mindset

## Target resume bullet

Implemented observability with Prometheus, Grafana, Loki, and alerting; rebuilt the cluster from code in a timed DR drill (RTO: N min).

This is a target. The recovery-time figure stays a placeholder until the drill is timed. It is not done yet.

## Notes

_None yet._

## Evidence

_None yet._
