# 🧠 Cybersecurity Knowledge Mind Map

**Visual Learning Reference** · Security+ · Network+ · Blue Team Level 1

A comprehensive, self-built visual knowledge map covering the core domains of cybersecurity — structured specifically around SOC analyst operations, threat detection, and defensive security practice.

---

## What This Is

A hand-built mind map created as a living study reference and knowledge consolidation tool during my transition into cybersecurity. Every branch has been researched, structured, and written from scratch — not copied from a template.

The map is built to reflect how a working SOC analyst actually thinks across domains, with deliberate **SOC Tie-in** callouts throughout each section connecting theory directly to real analyst workflows.

---

## Why I Built It

Most cybersecurity study materials are linear — courses, modules, chapters. Mind maps force you to understand **how concepts connect**, not just what they are individually.

Building this map required understanding *why* network segmentation relates to least privilege, why change management matters for incident investigation, and why IOAs outlast IOCs. It's also a reference I can use in real SOC work — not a diagram to look at once and forget.

---

## Domains Covered

### 🔐 Core Security Concepts
- CIA Triad & AAA (Authentication, Authorisation, Accounting)
- Zero Trust architecture — Never Trust, Always Verify
- Controls: Preventative, Detective, Corrective, Deterrent, Physical, Operational
- All Layers Defence model
- Risk concepts, assessment methodology & treatment (Avoid, Mitigate, Transfer, Accept)

### ⚠️ Threats
- **Threat Vectors:** Network, Web/App, Physical, Supply Chain, Wireless, Cloud
- **Threat Types:** Malware/Endpoint, Network, Social Engineering (inc. BEC), Wireless, Cloud/Virtual, Physical, Insider, Supply Chain, Emerging
- **Threat Actors:** Nation State, Hacktivists, Organised Crime, Unskilled Attackers, Inside Threat

### 🛡️ Defense Hardening
- Network segmentation & Zero Trust model
- Least privilege — RBAC/ABAC, PAM, Just-in-Time access
- Patch management lifecycle & tooling (WSUS/SCCM, Intune, Ansible, Qualys)
- Secure configurations — Windows (Group Policy, AppLocker), Linux (SELinux/AppArmor), CIS Benchmarks
- Endpoint protection — EDR, AV/NGAV, App Control, Host Firewall, Device Control, Email Hardening
- Cryptography & Encryption — Symmetric (AES), Asymmetric (RSA, ECC), Diffie-Hellman, DSA, Hashing (SHA), HMAC

### ⚙️ Security Operations
- **Threat Hunting** — IoC & IoA based, hypothesis-driven, MITRE ATT&CK framework integration
- **Logging & Monitoring** — SIEM sources, log normalisation, MTTD/MTTR, alert fatigue reduction
- **IAM & Authentication** — MFA, SSO, Federation, PAM, JIT access, service account monitoring
- **SOAR** — Security Orchestration, Automation & Response; Splunk SOAR, Palo Alto XSOAR, Tines
- **Endpoint Security** — AV/EDR, Device Control, Host Firewall, Email Client Hardening
- **Incident Response** — NIST 800-61: Preparation → Identification → Containment → Eradication → Recovery → Lessons Learned

### 🔄 SOC Workflows & Processes
- Alert triage — TP/FP/TN/FN classification, severity tiers (Critical → High → Medium → Low)
- Escalation paths — L1 → L2 → L3 criteria and handoff documentation
- Ticket lifecycle — Open → Assigned → Investigating → Contained → Resolved → Closed
- Playbooks — Phishing, Ransomware, Brute Force, Data Exfiltration
- Shift handover discipline

### 📋 Governance, Risk & Compliance (GRC)
- **Governance** — Policies, roles, CISO accountability, data classification, AUP
- **Risk Management** — Risk formula, quantitative vs qualitative, risk register, residual risk
- **Compliance** — GDPR, HIPAA, PCI-DSS, Privacy Act 1988, NDB scheme, APRA CPS 234
- **Frameworks & Standards** — NIST CSF, ISO 27001, CIS Controls v8, Essential Eight (ASD), SOC 2
- **Audit & Assessments** — Internal vs external, penetration testing, vulnerability assessment, gap analysis
- **Security Awareness** — Phishing simulations, training metrics, staff reporting culture
- **Change Management** — CAB process, change types, security impact assessment

### 🏗️ Design & Architecture
- All Layers Defence — Perimeter, Network, Host, Data, Application, User
- Risk concepts & treatment options
- Security-by-design principles

### 🎯 MITRE ATT&CK Framework
- Structure — 14 Tactics → Techniques → Sub-techniques (e.g. T1566.001)
- SOC usage — detection mapping, Navigator coverage heat-mapping, purple team exercises
- **MITRE D3FEND** — Defensive counterpart; maps defensive techniques to attacker techniques (Harden, Detect, Isolate, Deceive, Evict)

### ☁️ Cloud Security
- Shared Responsibility Model — IaaS vs PaaS vs SaaS
- Cloud misconfigurations — open S3 buckets, overpermissioned IAM roles, public snapshots
- CSPM tools — Prisma Cloud, Wiz, AWS Security Hub, Microsoft Defender for Cloud
- Cloud-native threats — SSRF → IMDS abuse, container escape, K8s RBAC misconfigs, CI/CD supply chain

### 🔍 Vulnerability Management
- CVE & CVSS v3.1 scoring — Base, Temporal, Environmental score bands
- CISA KEV list — always prioritise Known Exploited Vulnerabilities regardless of CVSS
- Scanning tools — Nessus, OpenVAS, Qualys, Rapid7 InsightVM
- Patch SLA targets — Critical 24–48hr, High 7 days, Medium 30 days, Low 90 days

### 🌐 Threat Intelligence
- Intelligence types — Strategic, Tactical, Operational, Technical
- IOCs vs IOAs — why IOAs are more durable for detection
- **Pyramid of Pain** — Hash → IP → Domain → Network/Host Artefacts → Tools → TTPs (hardest for attacker to change = most valuable for defenders)
- Feeds & platforms — VirusTotal, Shodan, AbuseIPDB, MISP, STIX/TAXII, Recorded Future

### 🧬 Digital Forensics & IR (DFIR)
- Order of volatility — RAM first → running processes → network state → disk → remote logs
- Chain of custody & write blockers — required for legal admissibility
- Memory forensics — Volatility, Rekall; detect injected code, rogue processes, credentials in RAM
- Disk imaging — FTK Imager, dd, Autopsy, EnCase; bit-for-bit with MD5/SHA-256 hash verification

---

## How to Use It

| Use Case | How It Helps |
|---|---|
| **Cert study** | Maps closely to Security+, BTL1, CySA+ domain structure |
| **Interview prep** | Each branch covers what hiring managers actually ask L1 candidates |
| **SOC reference** | SOC Tie-in callouts connect theory directly to analyst workflows |
| **Domain overview** | See how all security concepts connect, not just individual definitions |

---

## Status

🔄 **Living document** — updated as new domains are studied and as real-world SOC knowledge deepens.

| Domain | Status |
|---|---|
| Security Concepts | ✅ Complete |
| Threats | ✅ Complete |
| Defense Hardening | ✅ Complete |
| Security Operations | ✅ Complete |
| SOC Workflows & Processes | ✅ Complete |
| Governance, Risk & Compliance | ✅ Complete |
| Design & Architecture | ✅ Complete |
| MITRE ATT&CK & D3FEND | ✅ Complete |
| Cloud Security | ✅ Complete |
| Vulnerability Management | ✅ Complete |
| Threat Intelligence | ✅ Complete |
| Digital Forensics & IR (DFIR) | ✅ Complete |

---

## Related Projects

| Project | Description |
|---|---|
| [SOC Detection Engineering & Alert Improvement](https://github.com/MarshallSecOps/SOC-Detection-Engineering-Improvement) | Production-ready detection tuning across 4 high-volume alerts — 89.7% alert reduction, $2.89M annual savings, 100% TP retention |
| [SOC Alert Triage & Escalation Workflow](https://github.com/MarshallSecOps/SOC-Alert-Triage-Project) | Structured triage, investigation and playbook development using Splunk |
| [APT29 DFIR Investigation](https://github.com/MarshallSecOps/apt29-DFIR-Investigation) | End-to-end threat actor investigation reconstructed from raw Windows telemetry |

---

**Author:** Marshall  
**Target Role:** SOC Tier 1 / Tier 2 Analyst  
📍 Gold Coast, Australia · Open to remote and hybrid cybersecurity roles


