# Rahul's Cybersecurity Project Portfolio 🔐

I learn security by building it, breaking it, and writing up what happened. These projects cover the full loop: engineering an AI-assisted threat hunting tool, getting breached on purpose and responding like a real incident, and standing up a vulnerability management program from scratch.

Every repo has a full write-up with the queries, scripts and screenshots behind the claims. Take a look around.

---

## 🤖 AI-Powered Security Operations

### [AI Agentic SOC](https://github.com/Rahulpatnala-99999/ai-agentic-soc)

A threat hunting application that turns plain-English security questions into KQL, runs them against Microsoft Azure Log Analytics, and analyzes the telemetry for signs of compromise. Findings are mapped to MITRE ATT&CK with IOCs, confidence levels and recommended actions, and qualifying host findings can be isolated through Microsoft Defender.

- Query planning with table and field allow-list guardrails, so generated KQL stays inside approved data
- Quick mode for one-shot investigations, Advanced mode to review and edit the KQL before analysis
- Live progress streaming, searchable investigation history, and a password-protected API
- Device isolation behind an explicit confirmation step

**Built with:** React, Vite, Material UI, FastAPI, OpenAI API, Azure Monitor Query, Microsoft Defender for Endpoint, KQL

---

## 🚨 Threat Detection and Incident Response

### [Live Breach and Incident Response Honeypot](https://github.com/Rahulpatnala-99999/live-breach-and-incident-response-honeypot)

I built an internet-exposed Windows 11 and MySQL honeypot on Azure, wired it into Microsoft Sentinel and Defender for Endpoint, and wrote the detections **before** exposing it. Then I weakened it on purpose and let the internet find it.

Within days an attacker logged into MySQL as `root`, dropped three databases and left a Bitcoin ransom note, while the host took an RDP brute-force campaign. I isolated the device, investigated with KQL, and wrote the incident response report.

- Custom log pipeline: MySQL general log to Azure Monitor Agent to a Log Analytics table
- Six investigation hunts covering brute force, database destruction, process activity, outbound traffic and persistence
- Full attack timeline, root cause, MITRE ATT&CK mapping, IOCs and prioritized recommendations

**Built with:** Azure, Microsoft Sentinel, Microsoft Defender for Endpoint, Azure Monitor Agent, MySQL, KQL

---

## ⚠️ Vulnerability Management Projects

- **[Vulnerability Management Program Implementation](https://github.com/Rahulpatnala-99999/vulnerability-management-program)**: a simulated program built from zero, covering policy drafting, stakeholder buy-in, CAB approval, authenticated Tenable scans and six remediation rounds. Total vulnerabilities dropped 81% (26 to 5) and all criticals were resolved.
- **[Programmatic Vulnerability Remediations (PowerShell)](https://github.com/Rahulpatnala-99999/Programmatic-Vulnerability-Remediations)**: Windows 10 DISA STIG v3r2 findings from a Tenable Nessus scan, remediated with PowerShell scripts, each documented with verification steps and rollback instructions.

---

## 🛠️ Tools and Skills

**SIEM and EDR:** Microsoft Sentinel, Microsoft Defender for Endpoint
**Query and analysis:** KQL, MITRE ATT&CK, incident response reporting
**Vulnerability management:** Tenable / Nessus, DISA STIGs
**Automation and development:** Python, PowerShell, FastAPI, React
**Cloud:** Microsoft Azure

<hr/>

## 🤳 Connect With Me


<a href="https://linkedin.com/in/rahul-patnala"><img alt="LinkedIn" width="32px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linkedin/linkedin-original.svg" /></a>

