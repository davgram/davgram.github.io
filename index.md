---
layout: default
title: Projects
---

# Featured Projects

### Vulnerability Scanner Deployment  
[View on GitHub ↗](https://github.com/davgram/vuln-scanner-deployment)

Deploy a production-style vulnerability scanner and workflow.

**Stack:** Ubuntu Server · Greenbone/OpenVAS (or Nessus) · scheduled/credentialed scans · CVSS reporting  
**Highlights**
- Automated install and hardening (service user, TLS, firewall rules).
- **Targets:** Windows & Linux lab VMs, network appliances.
- **Jobs:** recurring scans, asset groups, differential reports, email alerts.
- **Outputs:** HTML/CSV reports, JSON exports, SIEM/syslog forwarding.
- **Process:** triage by CVSS, false-positive handling, ticketing handoff.

**See in repo:** install scripts (Bash/Ansible), scan policies, sample reports, SOP for remediation.

---

### Password Manager Hosted in Cloud  
[View on GitHub ↗](https://github.com/davgram/password-manager-cloud)

Self-hosted team password manager with backups and HTTPS.

**Stack:** Ubuntu VM · Docker (Vaultwarden/Bitwarden-compatible) · Nginx/Caddy · Let’s Encrypt  
**Highlights**
- One-command `docker-compose` deployment with persistent volumes.
- Automatic TLS via Let’s Encrypt; HTTP→HTTPS redirect; security headers.
- Daily encrypted backups (DB + attachments) to object storage.
- Hardening: non-root containers, UFW firewall, Fail2ban, audit logging.
- Restore procedure + rotation/incident playbook.

**See in repo:** `docker-compose.yml`, environment templates, backup/restore scripts, hardening checklist.

---

## Contact
[Download CV (PDF)](./Davide_Gramuglia_CV.pdf) · [GitHub](https://github.com/davgram) · [LinkedIn](https://www.linkedin.com/in/your-link) · [Email](mailto:your.email@example.com)
