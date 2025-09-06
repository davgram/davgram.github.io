---
layout: default
title: Projects
---

# Featured Projects

<!-- Certifications (stacked vertically under the header/tagline) -->
<div class="badge-col">
  <a class="btn badge" href="#" target="_blank" rel="noopener">CompTIA Security+</a>
  <a class="btn badge" href="#" target="_blank" rel="noopener">Blue Team Level 1 (BTL1)</a>
  <a class="btn badge" href="#" target="_blank" rel="noopener">TryHackMe SAL1</a>
</div>

### Vulnerability Scanner Deployment  
[View on GitHub ↗](https://github.com/davgram/vuln-scanner-deployment)

Deploy a production-style vulnerability scanner and build a remediation workflow.

**Stack:** Ubuntu Server · Greenbone/OpenVAS (or Nessus) · Credentialed scans · CVSS reporting  
**Highlights**
- Automated install & hardening (service user, TLS, firewall).
- **Targets:** Windows + Linux lab VMs and network appliances.
- **Jobs:** recurring schedules, asset groups, differential reports, email alerts.
- **Outputs:** HTML/CSV reports, JSON exports; optional SIEM/syslog forwarding.
- **Process:** triage by CVSS, false-positive handling, ticketing handoff.

**See in repo:** install scripts (Bash/Ansible), scan policies, SOPs, sample reports.

---

### Password Manager Hosted in Cloud  
[View on GitHub ↗](https://github.com/davgram/password-manager-cloud)

Self-hosted team password manager with backups, HTTPS, and hardening.

**Stack:** Ubuntu VM · Docker (Vaultwarden/Bitwarden-compatible) · Nginx/Caddy · Let’s Encrypt  
**Highlights**
- One-command `docker-compose` deployment with persistent volumes.
- Automatic TLS via Let’s Encrypt; HTTP→HTTPS redirect; strict security headers.
- Daily encrypted backups (DB + attachments) to object storage with retention.
- Hardening: non-root containers, UFW firewall, Fail2ban, audit logging.
- Restore procedure + rotation/incident playbook.

**See in repo:** `docker-compose.yml`, env templates, backup/restore scripts, hardening checklist.

---

## Contact
[Download CV (PDF)](./Davide_Gramuglia_CV.pdf) · [GitHub](https://github.com/davgram) · [LinkedIn](https://www.linkedin.com/in/your-link) · [Email](mailto:your.email@example.com)
