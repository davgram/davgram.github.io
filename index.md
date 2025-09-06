---
layout: default
title: Davide Gramuglia — Blue Team Portfolio
---

# Davide Gramuglia
**Blue-Team / SOC Analyst (entry level)** — network-focused, DFIR-curious.  
[**Download CV (PDF)**](./Davide_Gramuglia_CV.pdf) • [GitHub](https://github.com/davgram) • [LinkedIn](https://www.linkedin.com/in/your-link) • [Email](mailto:your.email@example.com)

---

## Featured Projects

### 1) Mini SOC Lab — Windows + Sysmon → Splunk & Elastic
Small, reproducible lab for log collection, hunting, and detections.

**Stack:** Win10 VM · Sysmon · Winlogbeat/UF → Splunk & Elastic · ATT&CK mapping  
**Highlights**
- Dashboards for **Sysmon EIDs 1/3/7/11/13/22** and Windows **4624/4625/4688/7045**  
- Detections for **LOLBINs**, **encoded PowerShell**, suspicious **parent/child chains**  
- Saved searches & alerts with documentation and triage steps

```spl
# Splunk: quick process creation triage (Sysmon EID 1)
index=wineventlog source="WinEventLog:Microsoft-Windows-Sysmon/Operational" EventCode=1
| stats count by Image, CommandLine, User, Computer | sort - count

