---
layout: default
---

**Davide Gramuglia — Blue Team / SOC Analyst (entry level)**  
Network-focused, DFIR-curious. Building detections, running small SOC labs, and writing clean incident notes.

[Portfolio repos](https://github.com/davgram) • [Download my CV (PDF)](./Davide_Gramuglia_CV.pdf) • [LinkedIn](https://www.linkedin.com/in/your-link) • [Email](mailto:your.email@example.com)

This site hosts my **cybersecurity résumé** and selected **blue-team projects**. Everything is minimalist and recruiter-friendly.

---

# Skills & Tools

**SIEM & Logs:** Splunk, Elastic (ELK), Windows Event Logs, Sysmon, Sigma  
**Network:** Zeek, Suricata, Wireshark, PCAP triage, DNS/HTTP/TLS basics  
**Endpoint/DFIR:** Volatility, Autoruns, Procmon/Procdump, LiME  
**Detection Eng.:** ATT&CK mapping, rule tuning, baselining, FP control  
**Scripting:** Python, PowerShell, regex for log parsing  
**Ops/Lab:** VMware/VirtualBox, Windows/Linux admin basics

## Featured Projects

> I like practical work: capture → parse → hunt → detect → document.

### Mini SOC Lab (Windows + Sysmon + Splunk/Elastic)

- Win10 VM with **Sysmon** shipping logs to **Splunk** and **Elastic**  
- Dashboards for process/network events, persistence, and script abuse  
- Detections for LOLBINs, encoded PowerShell, suspicious child-process trees

```spl
# Splunk: quick process creation triage (Sysmon EventCode=1)
index=wineventlog source="WinEventLog:Microsoft-Windows-Sysmon/Operational" EventCode=1
| stats count by Image, CommandLine, User, Computer
| sort - count
