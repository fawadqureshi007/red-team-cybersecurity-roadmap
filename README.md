# 🟥 Red Team Cybersecurity Roadmap 2026 — From Zero to Operator

> **A practical, red-team-first cybersecurity roadmap built from my own research, testing, study, and curation.** Learn the foundations first, then move toward reconnaissance, attack-surface analysis, web and network security, exploitation, Active Directory, cloud security, adversary simulation, detection awareness, reporting, and professional red-team tradecraft.

Welcome to my 2026 cybersecurity roadmap. I'm **Fawad Qureshi**, and I built this roadmap from my own research and practical learning journey.

This is **not** a generic checklist of certifications. My point of view is simple: if you want to become strong in offensive security, you need to understand **how systems actually work before you learn how to break them**.

The roadmap therefore starts with networking, Linux, Windows, programming, and security fundamentals, then progressively moves into reconnaissance, enumeration, web applications, vulnerabilities, exploitation concepts, privilege escalation, Active Directory, cloud, OPSEC, adversary simulation, and professional reporting.

> **My rule:** learn the technology → understand the attack surface → reproduce the weakness in an authorized lab → understand the defensive side → document what you learned.

⚠️ **Authorized-use only:** Everything in this roadmap is intended for legal labs, CTFs, your own systems, or systems where you have explicit permission to test. Never use these skills against real targets without authorization.


## 👤 Author & Research

**Author:** Fawad Qureshi

**Perspective:** Red Team / Offensive Security

**Research:** This roadmap is my own research, study, organization, and curation of cybersecurity learning resources. It is designed around an offensive-security mindset while still teaching the defensive concepts required to understand real-world attacks.

**Goal:** Build practical security capability rather than collecting certificates without understanding the underlying technology.

**Last reviewed:** 2026

---

## 🎯 How I Approach Cybersecurity

I follow an operator mindset:

1. **Understand the system** — networking, operating systems, authentication, applications, protocols.
2. **Map the attack surface** — assets, services, identities, trust relationships, exposed functionality.
3. **Enumerate carefully** — collect evidence before making assumptions.
4. **Validate weaknesses safely** — reproduce vulnerabilities in authorized environments.
5. **Understand impact** — privilege, access, data exposure, persistence, lateral movement, and business risk.
6. **Think like the defender** — logs, detections, controls, telemetry, and remediation.
7. **Document everything** — commands, observations, evidence, findings, and lessons learned.
8. **Repeat** — practical repetition is what turns knowledge into skill.

> **Red-team mindset:** Don't memorize tools. Learn what the tool is doing, why it works, what assumptions it makes, and how defenders can detect or stop it.

---

**Keywords:** cybersecurity roadmap, learn cybersecurity 2026, how to become a cybersecurity analyst, SOC analyst path, penetration testing roadmap, cloud security career, cybersecurity certifications, CompTIA Security+, OSCP, CISSP, SecAI+, AI security, free cybersecurity resources.

> **🆕 What's new in 2026:** AI-driven attacks *and* defenses (including autonomous "agentic" AI), identity-first and Zero Trust architecture, non-human/machine identity, post-quantum cryptography readiness, deepfake-enabled social engineering, and cloud-native security are reshaping the field. This edition reflects those shifts — and the certification landscape that changed alongside them.

---

## 🗂️ Table of Contents

1. [👤 Who This Roadmap Is For](#-who-this-roadmap-is-for)
2. [🚀 Foundation](#-foundation)
3. [🔎 Fundamentals](#-fundamentals)
4. [💻 Programming & Scripting](#-programming--scripting)
5. [🌐 Specialization Tracks](#-specialization-tracks)
6. [🤖 Emerging Areas (2026 Focus)](#-emerging-areas-2026-focus)
7. [🧪 Practical Experience & Labs](#-practical-experience--labs)
8. [📚 Continuous Learning](#-continuous-learning)
9. [📺 YouTube Channels](#-youtube-channels)
10. [💼 Job Roles & Salaries](#-job-roles--salaries)
11. [🔐 Improving Your Skills](#-improving-your-skills)
12. [💼 Finding a Job](#-finding-a-job)
13. [📜 Certifications](#-certifications)
14. [📅 6-Month Roadmap](#-6-month-roadmap)
15. [📈 Tips for Success](#-tips-for-success)
16. [📚 Recommended Books](#-recommended-books)
17. [🤝 Communities](#-communities)
18. [❓ Frequently Asked Questions](#-frequently-asked-questions)
19. [🤗 Contributing](#-contributing)

---

## 👤 Who This Roadmap Is For

This roadmap is primarily for people who want to understand **offensive security and red-team operations** from the ground up.

It is useful for:

- **Complete beginners** who want a structured path into cybersecurity.
- **Aspiring penetration testers** who want to understand the full workflow instead of learning isolated tools.
- **Red-team learners** building toward realistic adversary-simulation skills.
- **Blue-team / SOC analysts** who want to understand attacker behavior from the other side.
- **IT, networking, Linux, Windows, and cloud learners** who want to transition into security.
- **Security professionals** who want a broader offensive-security study plan.

### What You Should Expect

This roadmap is deliberately **hands-on and fundamentals-first**.

You will repeatedly encounter:

`Learn → Build → Enumerate → Analyze → Validate → Document → Defend`

You do **not** need to know everything before starting. You need consistency, curiosity, legal practice environments, and the willingness to understand the technology underneath every security technique.

### What This Roadmap Is NOT

- It is not a promise that you will become a professional pentester in a few months.
- It is not a list of “one-click hacking tools.”
- It is not a replacement for hands-on labs.
- It is not permission to attack systems you do not own or have authorization to test.
- It is not certification-first learning.

---

---

## 🚀 Phase 1 — Foundations: Learn the Machine Before You Attack It

Before you can defend systems, you need to understand how they work. These foundational skills — networking, operating systems, and core IT concepts — are non-negotiable. Hiring managers consistently cite weak fundamentals as the biggest gap in entry-level candidates.

- **Networking Basics** 🌐 — how devices share data and connect through networks.
  - [The Bits and Bytes of Computer Networking — Coursera (Google)](https://www.coursera.org/learn/computer-networking)
  - [Cisco Networking Academy (free courses)](https://www.netacad.com/)
  - [Professor Messer's free Network+ course (N10-009)](https://www.professormesser.com/network-plus/n10-009/n10-009-video/n10-009-training-course/)

- **Operating System Fundamentals** 🖥️ — how Windows and Linux internals work: process management, memory, permissions, the boot process.
  - [Operating System Concepts — Coursera](https://www.coursera.org/learn/os-pku)

- **Linux Essentials** 🐧 — most security tools (and most servers) run on Linux. Command-line fluency is mandatory.
  - [Linux Journey (free, interactive)](https://linuxjourney.com/)
  - [OverTheWire: Bandit (learn Linux through challenges)](https://overthewire.org/wargames/bandit/)
  - [Linux Essentials — LPI](https://www.lpi.org/our-certifications/linux-essentials-overview/)

- **TCP/IP Networking** 🌐 — the protocol stack the entire internet runs on.
  - [Beej's Guide to Network Programming (free)](https://beej.us/guide/bgnet/)
  - [TCP/IP Networking — Pluralsight](https://www.pluralsight.com/courses/tcp-ip-networking)

- **Introduction to Cybersecurity** 🔒 — start with the *why* and the big picture.
  - [ISC2 Certified in Cybersecurity (CC)](https://www.isc2.org/certifications/cc) — vendor-neutral entry cert. **Note:** the free "One Million Certified in Cybersecurity" program closed to new enrollments on **May 20, 2026**. The CC is now a standard paid exam (about **$199 + $50 annual maintenance fee**), and a **new exam outline takes effect September 1, 2026**.
  - [Introduction to Cyber Security Specialization — Coursera](https://www.coursera.org/specializations/intro-cyber-security)

- **CompTIA Network+** 📜 — the industry-recognized credential validating your networking knowledge.
  - [CompTIA Network+ official](https://www.comptia.org/certifications/network)

- **Virtualization Basics** 🌪️ — you'll spin up virtual labs constantly.
  - [VirtualBox (free)](https://www.virtualbox.org/)
  - [VMware Workstation (now free for personal *and* commercial use)](https://www.vmware.com/products/desktop-hypervisor/workstation-and-fusion)

---

## 🔎 Phase 2 — Security Fundamentals & Attacker Thinking

With the basics in place, dive into core security concepts and the tools security teams use every day.

- **Security Fundamentals**
  - [CompTIA Security+ — official](https://www.comptia.org/certifications/security) — the current exam is **SY0-701**. A successor (**SY0-801**, adding AI/LLM security content) is expected to preview in **late 2026**; SY0-701 stays valid and fully recognized, so most people should still take it now.
  - [Professor Messer's free Security+ training (SY0-701)](https://www.professormesser.com/security-plus/sy0-701/sy0-701-video/sy0-701-training-course/)
  - [Google Cybersecurity Professional Certificate — Coursera](https://www.coursera.org/professional-certificates/google-cybersecurity)

- **The CIA Triad & Core Principles** — Confidentiality, Integrity, Availability: the bedrock of every security decision.
  - [NIST Cybersecurity Framework 2.0](https://www.nist.gov/cyberframework)

- **Common Vulnerabilities** ⚠️
  - [OWASP Top 10 (web app risks)](https://owasp.org/www-project-top-ten/)
  - [OWASP API Security Top 10](https://owasp.org/www-project-api-security/)
  - [CWE Top 25 Most Dangerous Software Weaknesses](https://cwe.mitre.org/top25/)

- **Threat Modeling & Attacker Mindset**
  - [MITRE ATT&CK Framework](https://attack.mitre.org/) — the standard map of how real attackers operate. Learn it cold.
  - [MITRE D3FEND](https://d3fend.mitre.org/) — the defensive-countermeasures companion to ATT&CK.
  - [MITRE ATLAS](https://atlas.mitre.org/) — the ATT&CK-style knowledge base for attacks on **AI/ML systems** (increasingly essential in 2026).

- **Cybersecurity Frameworks** 📏
  - [NIST Cybersecurity Framework 2.0](https://www.nist.gov/cyberframework)
  - [CIS Critical Security Controls](https://www.cisecurity.org/controls)
  - [ISO/IEC 27001](https://www.iso.org/standard/27001)

- **Incident Response Fundamentals** 🚨
  - [NIST SP 800-61 Rev. 3 (April 2025) — Incident Response for Cybersecurity Risk Management](https://csrc.nist.gov/pubs/sp/800/61/r3/final) — fully rewritten to align with CSF 2.0's six Functions (Govern, Identify, Protect, Detect, Respond, Recover). This supersedes Rev. 2.
  - [SANS Reading Room — Incident Handling papers (free)](https://www.sans.org/white-papers/)

- **Introduction to Malware Analysis** 🦠
  - [Malware Unicorn — Reverse Engineering 101](https://malwareunicorn.org/workshops/re101.html)
  - [ANY.RUN sandbox (analyze samples in-browser)](https://any.run/)

- **Phishing & Social Engineering Awareness** 📧
  - [Social Engineering Framework — Security Through Education](https://www.social-engineer.org/framework/general-discussion/)
  - [PhishTank — known phishing sites](https://phishtank.org/)

- **Cryptography Basics** 🔐
  - [Cryptopals Crypto Challenges (free, hands-on)](https://cryptopals.com/)
  - [Khan Academy: Journey into Cryptography](https://www.khanacademy.org/computing/computer-science/cryptography)

- **Data Privacy & Compliance** 🔒
  - [GDPR overview](https://gdpr.eu/what-is-gdpr/)
  - [HIPAA basics](https://www.hhs.gov/hipaa/for-professionals/index.html)
  - [PCI DSS](https://www.pcisecuritystandards.org/)

---

## 💻 Phase 3 — Programming & Scripting for Operators

You don't need to be a software engineer, but you do need to read and write code. Automation, tooling, and analysis all live here.

- **Python** 🐍 — the lingua franca of security tooling.
  - [Automate the Boring Stuff with Python (free online)](https://automatetheboringstuff.com/)
  - [Python for Cybersecurity Specialization — Coursera](https://www.coursera.org/specializations/pythonforcybersecurity)

- **Bash & Shell Scripting** 🐚
  - [The Bash Guide](https://guide.bash.academy/)
  - [ShellCheck (lint your scripts)](https://www.shellcheck.net/)

- **PowerShell** 💠 — essential for Windows / Active Directory work.
  - [Microsoft PowerShell 101](https://learn.microsoft.com/en-us/powershell/scripting/learn/ps101/00-introduction)

- **Understanding code you'll see in the wild**
  - JavaScript (web exploitation, XSS)
  - SQL (injection attacks, database hardening)
  - C / C++ (memory corruption, deeper malware analysis)

- **Regular Expressions** — [RegexOne (interactive)](https://regexone.com/)

---

## 🌐 Phase 4 — Offensive Security & Specialization Tracks

After fundamentals, pick a track. Specialists tend to out-earn generalists, and most 2026 roles expect depth, not just breadth. Below are the major tracks with the certifications that signal expertise in each.

### 1. Security Operations / SOC Analyst (Blue Team) 🛡️
**You'll do:** monitor SIEM alerts, investigate incidents, respond to threats.
- [CompTIA Security+](https://www.comptia.org/certifications/security)
- [CompTIA CySA+](https://www.comptia.org/certifications/cybersecurity-analyst)
- [Blue Team Level 1 (BTL1)](https://www.securityblue.team/why-btl1)

### 2. Penetration Testing / Red Team 💻
**You'll do:** simulate attacks to find weaknesses before real adversaries do.
- [CompTIA PenTest+](https://www.comptia.org/certifications/pentest)
- [INE eJPT (great entry-level practical)](https://security.ine.com/certifications/ejpt-certification/)
- [Certified Ethical Hacker (CEH)](https://www.eccouncil.org/programs/certified-ethical-hacker-ceh/)
- [OffSec PEN-200 → OSCP / OSCP+](https://www.offsec.com/courses/pen-200/) — the gold-standard hands-on cert. Since **November 2024**, passing awards both the lifetime **OSCP** and the 3-year **OSCP+**; the exam now includes a mandatory Active Directory "assumed compromise" set and no longer awards bonus points.

### 3. Incident Response & Digital Forensics 🔍
**You'll do:** investigate breaches, recover evidence, write up what happened.
- [GIAC Certified Incident Handler (GCIH)](https://www.giac.org/certifications/certified-incident-handler-gcih/)
- [GIAC Certified Forensic Analyst (GCFA)](https://www.giac.org/certifications/certified-forensic-analyst-gcfa/)

### 4. Governance, Risk & Compliance (GRC) 📝
**You'll do:** map controls to frameworks, manage audits, translate security to business.
- [ISACA CISA — Certified Information Systems Auditor](https://www.isaca.org/credentialing/cisa)
- [ISACA CRISC — Risk and Information Systems Control](https://www.isaca.org/credentialing/crisc)
- [ISO/IEC 27001 Lead Auditor (PECB)](https://www.pecb.com/en/education-and-certification-for-individuals/iso-iec-27001)

### 5. Security Architecture & Leadership 🏛️
**You'll do:** design enterprise security, make build-vs-buy calls, run programs.
- [ISC2 CISSP](https://www.isc2.org/certifications/cissp)
- [ISC2 CISSP-ISSAP (Architecture concentration)](https://www.isc2.org/certifications/issap)
- [ISACA CISM — Information Security Manager](https://www.isaca.org/credentialing/cism)
- [CompTIA SecurityX (the successor to CASP+)](https://www.comptia.org/certifications/comptia-advanced-security-practitioner) — vendor-neutral advanced/architect-level cert. Existing CASP+ holders transition automatically, no retake required.

### 6. Cloud Security ☁️
The fastest-growing specialization. Almost every org runs hybrid/multi-cloud now.
- [ISC2 CCSP](https://www.isc2.org/certifications/ccsp)
- [AWS Certified Security – Specialty](https://aws.amazon.com/certification/certified-security-specialty/)
- [Microsoft SC-100: Cybersecurity Architect Expert](https://learn.microsoft.com/en-us/credentials/certifications/cybersecurity-architect-expert/)
- [Google Cloud Professional Cloud Security Engineer](https://cloud.google.com/learn/certification/cloud-security-engineer)

### 7. Application Security (AppSec) / DevSecOps 📱
- [GIAC Web Application Penetration Tester (GWAPT)](https://www.giac.org/certifications/web-application-penetration-tester-gwapt/)
- [OffSec WEB-200 → OSWA](https://www.offsec.com/courses/web-200/)
- [Certified DevSecOps Professional (CDP)](https://www.practical-devsecops.com/certified-devsecops-professional/)

### 8. Identity & Access Management (IAM) 🪪
Identity is the new perimeter in 2026 — and **non-human / machine identity** (service accounts, API keys, and AI agents) is now one of the fastest-growing attack surfaces.
- [Microsoft SC-300: Identity and Access Administrator](https://learn.microsoft.com/en-us/credentials/certifications/identity-and-access-administrator/)
- [Okta certifications](https://www.okta.com/services/training/certification/)

### 9. AI Security 🧠 (new track)
Securing AI systems — and using AI safely inside security operations — is now its own career path.
- [CompTIA SecAI+ (CY0-001)](https://www.comptia.org/en-us/certifications/secai/) — launched **February 17, 2026**, the first vendor-neutral certification focused on securing AI systems *and* leveraging AI in security operations. Recommended after Security+/CySA+/PenTest+.
- Free foundations: [OWASP Top 10 for LLM Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/), [MITRE ATLAS](https://atlas.mitre.org/), and the [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework).

---

## 🤖 Phase 5 — Modern Attack Surface: AI, Cloud, Identity & Zero Trust

These aren't fringe topics anymore — they appear in mainstream job descriptions. Building familiarity here will set you apart.

- **AI Security & Adversarial ML** 🧠 — how attackers exploit AI systems (prompt injection, training-data poisoning, model extraction, jailbroken LLMs) and how defenders use AI for detection. In 2026, **agentic AI** — autonomous agents that reason, plan, and act — is being used on *both* sides: to automate parts of the attack kill chain, and to accelerate SOC triage and investigation. "Autonomous agent hijacking" is now a recognized attack category.
  - [OWASP Top 10 for LLM Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
  - [MITRE ATLAS — adversarial threat landscape for AI systems](https://atlas.mitre.org/)
  - [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework)

- **Deepfakes & AI-Enabled Social Engineering** 🎭 — voice- and video-cloning are now routinely used in fraud and business-email-compromise. The defensive shift is toward *contextual verification* (out-of-band callbacks, code words, verifying intent) rather than trying to spot fakes visually.

- **Non-Human Identity (NHI) & Machine Identity** 🤖🪪 — service accounts, API keys, secrets, and AI-agent credentials now vastly outnumber human identities and are a top lateral-movement vector. Expect to see NHI governance in more job descriptions.

- **Zero Trust Architecture** 🚧 — "never trust, always verify." The replacement for perimeter-based security, now extended to devices, workloads, APIs, and AI systems.
  - [NIST SP 800-207 Zero Trust Architecture](https://csrc.nist.gov/pubs/sp/800/207/final)
  - [CISA Zero Trust Maturity Model](https://www.cisa.gov/zero-trust-maturity-model)

- **Post-Quantum Cryptography (PQC)** 🔮 — NIST finalized its first three quantum-resistant standards in **August 2024**: **ML-KEM (FIPS 203)** for key exchange, **ML-DSA (FIPS 204)** and **SLH-DSA (FIPS 205)** for signatures. **HQC** was selected as a backup KEM in **March 2025**, and a FALCON-based signature standard (**FIPS 206**) is in progress. "Harvest now, decrypt later" attacks make migration urgent.
  - [NIST Post-Quantum Cryptography Project](https://csrc.nist.gov/projects/post-quantum-cryptography)

- **Supply Chain & Software Bill of Materials (SBOM)**
  - [CISA SBOM resources](https://www.cisa.gov/sbom)
  - [SLSA — Supply-chain Levels for Software Artifacts](https://slsa.dev/)

- **Container & Kubernetes Security**
  - [OWASP Kubernetes Security Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Kubernetes_Security_Cheat_Sheet.html)
  - [CIS Kubernetes Benchmark](https://www.cisecurity.org/benchmark/kubernetes)

- **OT / ICS Security** ⚙️ — securing industrial control systems and critical infrastructure. A high-paying specialization with a large talent gap.
  - [SANS Industrial Control Systems (ICS) training](https://www.sans.org/industrial-control-systems-security/)

---

## 🧪 Phase 6 — Labs, CTFs & Building Your Own Range

Certifications open doors; hands-on skills get you hired. Hiring managers consistently say practical experience matters more than credentials alone.

- **TryHackMe** 🔐 — guided, beginner-friendly rooms — [tryhackme.com](https://tryhackme.com/)
- **Hack The Box** 🕵️ — more advanced, CTF-style — [hackthebox.com](https://www.hackthebox.com/)
- **OverTheWire** ⚔️ — classic wargames, great for Linux — [overthewire.org/wargames](https://overthewire.org/wargames/)
- **VulnHub** 🏴‍☠️ — downloadable vulnerable VMs — [vulnhub.com](https://www.vulnhub.com/)
- **PortSwigger Web Security Academy** 🌐 — best free web-app security training, by the makers of Burp Suite — [portswigger.net/web-security](https://portswigger.net/web-security)
- **picoCTF** 🚩 — free, beginner-friendly CTF platform — [picoctf.org](https://picoctf.org/)
- **CTFtime** 📅 — calendar of running CTF competitions worldwide — [ctftime.org](https://ctftime.org/)
- **Blue Team Labs Online** 🔵 — defender-focused challenges — [blueteamlabs.online](https://blueteamlabs.online/)
- **LetsDefend** — SOC analyst simulation — [letsdefend.io](https://letsdefend.io/)
- **Proving Grounds (OffSec)** — OSCP-like practice — [offsec.com/labs](https://www.offsec.com/labs/individual/)
- **RangeForce** — interactive defense labs — [rangeforce.com](https://www.rangeforce.com/)

### 🟥 My Recommended Red-Team Workflow

For most practical engagements and labs, think in this order:

```text
1. Scope & Authorization
        ↓
2. Reconnaissance
        ↓
3. Enumeration
        ↓
4. Attack-Surface Mapping
        ↓
5. Vulnerability Analysis
        ↓
6. Controlled Validation
        ↓
7. Privilege / Access Analysis
        ↓
8. Lateral-Movement Concepts
        ↓
9. Objective / Impact Validation
        ↓
10. Evidence Collection
        ↓
11. Reporting & Remediation
```

The exact workflow changes by engagement, but the principle stays the same: **enumerate before exploiting, understand before automating, and document before moving on.**

---

### Build a Home Lab
A home lab is one of the best portfolio builders. Common setups:
- **Active Directory lab** — a domain controller + a couple of Windows clients + a Kali attacker.
- **Detection lab** — the [DetectionLab project](https://github.com/clong/DetectionLab) ships a pre-built Splunk + Velociraptor + Sysmon environment. (Check the repo's current status/notes before relying on it.)
- **SOC-in-a-box** — [Security Onion](https://securityonionsolutions.com/), the ELK/Elastic Stack, or [Wazuh](https://wazuh.com/).

---

## 🧠 Red-Team Skill Matrix

Use this as a self-assessment rather than a checklist of tools.

| Area | Beginner | Intermediate | Advanced |
|---|---|---|---|
| Networking | TCP/IP, DNS, HTTP, ports | Routing, segmentation, packet analysis | Complex enterprise networks |
| Linux | CLI, permissions, processes | Services, logs, scripting | Privilege/security internals |
| Windows | Users, services, PowerShell | AD basics, Kerberos, Windows internals | Enterprise identity attack paths |
| Web | HTTP, cookies, auth | OWASP Top 10, Burp Suite | Complex application/API testing |
| Recon | Asset discovery concepts | Enumeration and attack-surface mapping | Large-scope external recon |
| Exploitation | Understand vulnerabilities | Reproduce vulnerabilities in labs | Chain weaknesses responsibly |
| Privilege Escalation | Basic concepts | Linux/Windows enumeration | Complex escalation paths |
| Active Directory | Domains/users/groups | Authentication and trust concepts | Attack-path analysis |
| Cloud | IAM/storage/network basics | Cloud attack surfaces | Multi-account / hybrid environments |
| Scripting | Python/Bash/PowerShell basics | Automation | Custom security tooling |
| Reporting | Clear notes | Professional findings | Executive + technical reporting |
| OPSEC | Understand exposure | Reduce unnecessary noise | Engagement-aware operational discipline |

> **Important:** A tool-heavy skillset without fundamentals is fragile. My priority is understanding the system first and the tool second.

---

## 📚 Continuous Learning

Cybersecurity changes faster than any other IT discipline. Staying current is part of the job.

- **The Hacker News** 👨‍💻 — [thehackernews.com](https://thehackernews.com/)
- **BleepingComputer** 💻 — [bleepingcomputer.com](https://www.bleepingcomputer.com/)
- **Krebs on Security** 🔍 — [krebsonsecurity.com](https://krebsonsecurity.com/)
- **Dark Reading** 📰 — [darkreading.com](https://www.darkreading.com/)
- **CyberScoop** 🌐 — [cyberscoop.com](https://cyberscoop.com/)
- **Risky Business** 🎙️ (podcast) — [risky.biz](https://risky.biz/)
- **TLDR Sec** 📩 (newsletter) — [tldrsec.com](https://tldrsec.com/)
- **SANS Internet Storm Center** 🌪️ — [isc.sans.edu](https://isc.sans.edu/)
- **CISA Advisories** 🚨 — [cisa.gov/news-events/cybersecurity-advisories](https://www.cisa.gov/news-events/cybersecurity-advisories)
- **Schneier on Security** 🔐 — [schneier.com](https://www.schneier.com/)

### Reddit Communities
[r/cybersecurity](https://www.reddit.com/r/cybersecurity/) · [r/netsec](https://www.reddit.com/r/netsec/) · [r/AskNetsec](https://www.reddit.com/r/AskNetsec/) · [r/blueteamsec](https://www.reddit.com/r/blueteamsec/) · [r/redteamsec](https://www.reddit.com/r/redteamsec/)

### People to Follow
Brian Krebs · Bruce Schneier · SwiftOnSecurity · Marcus Hutchins (MalwareTech) · Katie Nickels (threat intel) · John Hammond.

---

## 📺 YouTube Channels

- [John Hammond](https://www.youtube.com/@_JohnHammond) — CTFs, malware analysis, practical projects
- [NetworkChuck](https://www.youtube.com/@NetworkChuck) — networking, Linux, cloud, fun and accessible
- [Professor Messer](https://www.youtube.com/@professormesser) — complete free CompTIA training
- [The Cyber Mentor (TCM Security)](https://www.youtube.com/@TCMSecurityAcademy) — ethical hacking and pentesting
- [IppSec](https://www.youtube.com/@ippsec) — Hack The Box walkthroughs (gold standard)
- [LiveOverflow](https://www.youtube.com/@LiveOverflow) — deep technical hacking content
- [HackerSploit](https://www.youtube.com/@HackerSploit) — penetration testing tutorials
- [David Bombal](https://www.youtube.com/@davidbombal) — networking, security, career advice
- [Hak5](https://www.youtube.com/@hak5) — hacking gear and techniques
- [STÖK](https://www.youtube.com/@STOKfredrik) — bug bounty hunting
- [InsiderPhD](https://www.youtube.com/@InsiderPhD) — bug bounty and API security
- [LowLevelLearning](https://www.youtube.com/@LowLevelLearning) — low-level systems and security

---

## 💼 Job Roles & Salaries

The ranges below are **2025–2026 estimates** and vary widely by experience, location, industry, and certifications. Always cross-check with current sources before making decisions.

| Job Role                  | Avg. Salary (PHP) | Avg. Salary (USD)  | Avg. Salary (AUD) |
|---------------------------|-------------------|--------------------|-------------------|
| SOC Analyst (Tier 1)      | ₱600,000          | $55,000–$75,000    | AU$70,000         |
| Security Analyst          | ₱850,000          | $75,000–$95,000    | AU$95,000         |
| Network Security Engineer | ₱1,200,000        | $95,000–$120,000   | AU$110,000        |
| Penetration Tester        | ₱1,100,000        | $90,000–$130,000   | AU$115,000        |
| Incident Responder        | ₱1,300,000        | $100,000–$140,000  | AU$125,000        |
| Forensic Analyst          | ₱1,150,000        | $85,000–$115,000   | AU$105,000        |
| Malware Analyst           | ₱1,400,000        | $100,000–$140,000  | AU$120,000        |
| Cloud Security Engineer   | ₱1,500,000        | $120,000–$160,000  | AU$140,000        |
| AI Security Engineer      | ₱1,600,000        | $130,000–$180,000  | AU$150,000        |
| Security Consultant       | ₱1,600,000        | $110,000–$160,000  | AU$130,000        |
| GRC Analyst               | ₱1,000,000        | $85,000–$115,000   | AU$105,000        |
| Security Architect        | ₱2,200,000        | $140,000–$200,000  | AU$170,000        |
| CISO                      | ₱4,000,000+       | $200,000–$400,000+ | AU$250,000+       |

### Verify current numbers here
- **Philippines:** [JobStreet](https://www.jobstreet.com.ph/), [PayScale Philippines](https://www.payscale.com/research/PH/Country=Philippines/Salary), [Kalibrr](https://www.kalibrr.com/)
- **United States:** [BLS Occupational Outlook Handbook](https://www.bls.gov/ooh/computer-and-information-technology/information-security-analysts.htm), [Glassdoor](https://www.glassdoor.com/), [Levels.fyi](https://www.levels.fyi/)
- **Australia:** [SEEK Salary Guide](https://www.seek.com.au/career-advice/page/salary-guide), [Hays Salary Guide](https://www.hays.com.au/salary-guide)

> **Market note (2026):** the global cybersecurity workforce gap remains large (commonly cited around **4+ million** unfilled roles), and **AI-security** roles are among the fastest-growing. Demand is strong, but entry-level competition has tightened — hands-on skills and a visible portfolio matter more than ever.

---

## 🔐 Improving Your Skills

1. **Practice secure online behavior** 🕵️
   - Use unique passwords with a password manager (Bitwarden, 1Password).
   - Enable multi-factor authentication everywhere — prefer hardware keys (YubiKey) or passkeys over SMS.
   - Be cautious about oversharing personal info online.

2. **Keep everything updated** 🔄 — auto-update your OS, browser, and apps; subscribe to vendor security advisories for tools you rely on.

3. **Secure your home network** 🛡️ — use WPA3 where possible, change default router credentials, segment IoT devices onto a guest network, and consider pfSense/OPNsense for serious labs.

4. **Educate yourself daily** 📚 — 15 minutes of news plus one TryHackMe room a day adds up fast.

5. **Use security tools** 🔧 — a VPN on untrusted networks, reputable EDR/antivirus, a password manager (mandatory), and DNS filtering (NextDNS, Cloudflare 1.1.1.1 for Families).

6. **Practice hands-on** 💻 — CTFs, home labs, write-ups. Document everything on GitHub — your portfolio is your proof.

7. **Join communities** 🌐 — Discord servers, Reddit, local DEF CON groups, OWASP and ISC2 chapters.

8. **Self-audit regularly** 🔍 — review your digital footprint quarterly and run [Have I Been Pwned](https://haveibeenpwned.com/) checks.

---

## 💼 Finding a Job

### 1. Build your portfolio
A resume tells; a portfolio shows. At minimum: a clean GitHub with lab and CTF write-ups, a technical blog (Medium, Hashnode, or self-hosted), and documented home-lab projects.

### 2. Tailor your resume
Use keywords from the job description (ATS systems screen aggressively), quantify wins ("reduced false-positive alerts by 30%"), and put relevant certs up top.

### 3. Apply broadly — especially to adjacent roles
You won't land Senior Pentester first. Realistic entry points: SOC Analyst Tier 1, Junior Security Analyst, IT Support → Security pivot, Help Desk → SOC pivot, GRC Analyst (often an easier entry for non-tech backgrounds), and internships/apprenticeships.

### 4. Job boards
[LinkedIn](https://www.linkedin.com/) · [Indeed](https://www.indeed.com/) · [Glassdoor](https://www.glassdoor.com/) · [CyberSecJobs](https://www.cybersecjobs.com/) · [InfoSec Jobs](https://infosec-jobs.com/) · [JobStreet (PH/SEA)](https://www.jobstreet.com/) · [Kalibrr (PH)](https://www.kalibrr.com/) · [Wellfound (startups)](https://wellfound.com/)

### 5. Network intentionally
Attend conferences (DEF CON, BSides, RSA, ROOTCON in PH), local meetups, and OWASP chapter events. On LinkedIn, comment thoughtfully — don't just spam connections.

### 6. Prepare for interviews
Common technical topics: networking (OSI/TCP), the cyber kill chain, MITRE ATT&CK, common attacks (XSS, SQLi, phishing), and IR basics. Behavioral: "tell me about a time you handled a difficult problem." Practical: many companies use scenario-based interviews or take-home labs.

### 7. Stay persistent
Track applications in a spreadsheet, ask for feedback on rejections, and keep learning while you apply.

---

## 📜 Certifications

Certifications build credibility, validate knowledge, and unlock job filters — but they don't replace experience. Be strategic about which ones you pursue.

### Entry-Level (start here)

- **CompTIA Security+ (SY0-701)** — [comptia.org/certifications/security](https://www.comptia.org/certifications/security)
  Appears in a large share of entry-level postings and satisfies the DoD 8140 baseline. The most universally useful first cert. (Successor **SY0-801** with AI content is expected to preview in late 2026; a current Security+ stays valid for three years regardless of version.)
- **Google Cybersecurity Professional Certificate** — [Coursera](https://www.coursera.org/professional-certificates/google-cybersecurity)
  Great for career switchers; budget-friendly with hands-on labs.
- **ISC2 Certified in Cybersecurity (CC)** — [isc2.org/certifications/cc](https://www.isc2.org/certifications/cc)
  Vendor-neutral and foundational. The free "One Million Certified" program **closed to new enrollments on May 20, 2026**; the CC is now a standard paid exam (~$199 + $50 AMF), with a **new exam outline effective September 1, 2026**.
- **CompTIA Network+** — [comptia.org/certifications/network](https://www.comptia.org/certifications/network)
  Networking foundation. Recommended before Security+ if you lack a networking background.

### Intermediate (after a year or two)

- **CompTIA CySA+** — [comptia.org/certifications/cybersecurity-analyst](https://www.comptia.org/certifications/cybersecurity-analyst) — best second cert for SOC/blue-team careers.
- **CompTIA PenTest+** — [comptia.org/certifications/pentest](https://www.comptia.org/certifications/pentest) — bridge to offensive security before OSCP.
- **CompTIA SecAI+ (CY0-001)** — [comptia.org/en-us/certifications/secai](https://www.comptia.org/en-us/certifications/secai/) — launched **Feb 17, 2026**; the first vendor-neutral AI-security cert. Builds on Security+/CySA+/PenTest+ and covers securing AI systems, AI-assisted security operations, and AI governance/risk/compliance.
- **Certified Ethical Hacker (CEH)** — [eccouncil.org](https://www.eccouncil.org/programs/certified-ethical-hacker-ceh/) — HR-friendly but criticized as theory-heavy; often required for government roles.
- **INE eJPT** — [security.ine.com](https://security.ine.com/certifications/ejpt-certification/) — affordable, practical entry to pentesting.

### Advanced / Specialist

- **OSCP / OSCP+ (OffSec)** — [offsec.com/courses/pen-200](https://www.offsec.com/courses/pen-200/) — gold standard for hands-on pentesting. OSCP is lifetime; **OSCP+** carries a 3-year validity (renewable via the OffSec CPE program, a recert exam, or another qualifying OffSec exam). Both are awarded on passing.
- **CompTIA SecurityX (formerly CASP+)** — [comptia.org](https://www.comptia.org/certifications/comptia-advanced-security-practitioner) — advanced/architect-level; CASP+ holders transition automatically.
- **GIAC GCIH / GSEC / GCFA / GPEN / GWAPT** — [giac.org/certifications](https://www.giac.org/certifications/) — highly respected but expensive (typically paired with SANS training).
- **ISC2 CISSP** — [isc2.org/certifications/cissp](https://www.isc2.org/certifications/cissp) — the leadership/architecture gold standard. Requires 5 years' experience.
- **ISC2 CCSP** — [isc2.org/certifications/ccsp](https://www.isc2.org/certifications/ccsp) — cloud security expert. Check ISC2 for the current exam outline before scheduling.
- **ISACA CISA / CISM / CRISC** — [isaca.org](https://www.isaca.org/credentialing/cisa) — audit, management, and risk; the GRC gold standards.
- **AWS Certified Security – Specialty** — [aws.amazon.com](https://aws.amazon.com/certification/certified-security-specialty/)
- **Microsoft SC-100 Cybersecurity Architect Expert** — [learn.microsoft.com](https://learn.microsoft.com/en-us/credentials/certifications/cybersecurity-architect-expert/)

> **A practical path for most beginners:**
> Google Cybersecurity Cert → Security+ → CySA+ (or PenTest+) → then a track cert (OSCP+ for offense, CCSP/SC-100 for cloud, CISA/CISM for GRC, SecAI+ for AI) → CISSP once you have the experience.

---

## 📅 6-Month Roadmap

A realistic plan. Adjust the pace to your schedule — full-time learners can compress this; nights/weekends learners may stretch to 9–12 months.

| Month       | Focus Area                        | Activities                                                                                                              | Resources                                                                                                                                     |
|-------------|-----------------------------------|------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|
| **Month 1** | Networking + Linux                | Set up a home lab in VirtualBox; install Ubuntu and Kali; complete networking basics; practice on the Linux CLI         | [Cisco NetAcad](https://www.netacad.com/), [Linux Journey](https://linuxjourney.com/), [OverTheWire Bandit](https://overthewire.org/wargames/bandit/) |
| **Month 2** | Security fundamentals + CIA triad | Begin Security+ study; learn the CIA triad, AAA, common threats; skim NIST CSF 2.0                                       | [Professor Messer Security+](https://www.professormesser.com/security-plus/sy0-701/sy0-701-video/sy0-701-training-course/), [NIST CSF](https://www.nist.gov/cyberframework) |
| **Month 3** | Threats, vulns & MITRE            | Study OWASP Top 10 and MITRE ATT&CK; read recent breach case studies; learn ransomware, phishing, supply-chain, AI threats | [OWASP Top 10](https://owasp.org/www-project-top-ten/), [MITRE ATT&CK](https://attack.mitre.org/), [Krebs on Security](https://krebsonsecurity.com/) |
| **Month 4** | Hands-on tools                    | Wireshark, Nmap, Burp Suite, Metasploit, basic Splunk/ELK; start the TryHackMe beginner path                            | [TryHackMe](https://tryhackme.com/), [Wireshark](https://www.wireshark.org/), [PortSwigger Academy](https://portswigger.net/web-security)      |
| **Month 5** | Practical skills + projects       | Take the Security+ exam; build out your home lab (AD or SOC); complete your first CTFs; document everything on GitHub    | [Security+](https://www.comptia.org/certifications/security), [DetectionLab](https://github.com/clong/DetectionLab), [picoCTF](https://picoctf.org/), [CTFtime](https://ctftime.org/) |
| **Month 6** | Specialize + network              | Pick a track (SOC, pentest, cloud, GRC, AI security); attend a virtual conference or local meetup; polish LinkedIn; start applying | [BSides](http://www.securitybsides.com/), [LinkedIn](https://www.linkedin.com/), [r/cybersecurity](https://www.reddit.com/r/cybersecurity/)   |

---

## 📈 Tips for Success

- **Build a portfolio** — a GitHub repo with documented labs, CTF write-ups, and tools you've written often beats certifications in technical interviews.
- **Stay updated** 🔄 — subscribe to 2–3 newsletters *max* (avoid overload). [Risky Business](https://risky.biz/), [TLDR Sec](https://tldrsec.com/), and [BleepingComputer](https://www.bleepingcomputer.com/) are great starts.
- **Master core tools** 🔧 — Wireshark, Nmap, Burp Suite, Metasploit, Splunk, the Linux CLI, and basic SIEM querying appear in nearly every job description.
- **Develop soft skills** — communication separates senior people from technicians. Practice writing clear reports and explaining technical concepts to non-technical stakeholders.
- **Find a mentor** — ISC2 chapters, meetups, and thoughtful LinkedIn outreach. Most professionals will give 30 minutes to someone making genuine effort.
- **Do CTFs** 🚩 — pick one per month from [CTFtime](https://ctftime.org/). Even failing teaches a lot.
- **Ethics first** — never use your skills on systems you don't have written permission to test. One unethical act can end a security career.
- **Contribute to open source** 🛠️ — bug reports, docs, and small fixes are great resume material.
- **Embrace "Try Harder"** — persistence beats genius. Most senior pros got there by being stubborn, not brilliant.

---

## 📚 Recommended Books

- *The Web Application Hacker's Handbook* — Dafydd Stuttard & Marcus Pinto
- *Hacking: The Art of Exploitation* — Jon Erickson
- *The Tangled Web* — Michał Zalewski
- *Practical Malware Analysis* — Sikorski & Honig
- *Cybersecurity Essentials* — Charles J. Brooks et al. (great intro)
- *Sandworm* — Andy Greenberg (nation-state threats)
- *Countdown to Zero Day* — Kim Zetter (the Stuxnet story)
- *The Cuckoo's Egg* — Cliff Stoll (a classic)
- *Permanent Record* — Edward Snowden
- *Click Here to Kill Everybody* — Bruce Schneier
- *Blue Team Handbook* — Don Murdoch
- *RTFM / BTFM* (Red/Blue Team Field Manuals) — Ben Clark / Alan White (cheat-sheet style)

---

## 🤝 Communities

- [OWASP](https://owasp.org/) — open web application security; local chapters worldwide
- [DEF CON Groups](https://defcongroups.org/) — local hacker meetups
- [BSides](http://www.securitybsides.com/) — community-driven conferences globally
- [ISC2 Chapters](https://www.isc2.org/chapters)
- [ISACA Chapters](https://engage.isaca.org/home)
- **Philippines:** [ROOTCON](https://www.rootcon.org/) — the premier PH hacking conference
- **Discord:** TCM Security, John Hammond, NetworkChuck, and the official Hack The Box community servers

---
## ❓ Frequently Asked Questions

### How do I start cybersecurity with no experience?

Learn **networking, Linux, Windows, and basic scripting** first. Then practice daily in legal labs like TryHackMe, Hack The Box, and PortSwigger. Don't just watch tutorials — **solve machines and figure out why things work**.

### Do I need certifications?

No. Certifications can help with getting interviews, but **skills matter more for practical security work**. Build labs, solve challenges, document your work, and learn how systems actually work.

### How much coding do I need?

You don't need to be a developer. Learn enough **Python, Bash, and PowerShell** to understand scripts, modify them, automate tasks, and build small tools.

### Can I become a red teamer in 6 months?

You can build a strong foundation in 6 months, but becoming genuinely good takes much longer. **Red teaming is a continuous learning process.**

### What does job-ready actually mean?

You should be able to take an unfamiliar system, **enumerate it, investigate weaknesses, troubleshoot problems, document your findings, and explain the impact** without depending on a walkthrough for every step.

### Are CTFs enough?

No. CTFs are great for technical practice, but real engagements also involve **scope, authorization, documentation, reporting, and business impact**.

### Do I need Kali Linux?

No. Kali is useful, but it doesn't make you a hacker. **Understand the underlying technology first; tools come second.**

### What's the biggest beginner mistake?

**Tool collecting instead of skill building.** Don't memorize hundreds of commands. Learn why you're running something and what information you are trying to obtain.

### How do I know I'm improving?

When you get stuck, instead of immediately looking for a walkthrough, you start thinking: **"What can I test, research, or investigate next?"** That's real progress.

### What's the reality of red teaming?

It's not just exploiting machines. A lot of the work is **recon, enumeration, research, troubleshooting, scripting, documentation, and thinking carefully about what to do next.**

### What's the best mindset?

**Learn → Practice → Break → Investigate → Understand → Document → Repeat.**

Practice only on systems you own or have explicit permission to test.


---

## 🤗 Contributing

Contributions are welcome! If you spot a broken link, an outdated fact, or have a resource to add, please [open an issue or a pull request](https://github.com/carlcastanas/Cybersecurity-Roadmap/pulls). Please keep resources free or clearly labeled, and prefer official/canonical sources.

---

## 👤 Author

**Fawad Qureshi**
*CEO & Founder — Codensec Security*
🌐 **[codensec.com](https://codensec.com)**


This roadmap represents my own research, learning, organization, and curation of cybersecurity resources from a **red-team / offensive-security perspective**.

If you find an outdated link, incorrect information, or a useful resource that should be added, open an issue or pull request with the relevant details.


---

## 🕒 Last Updated

- **Timezone:** Pakistan Standard Time (GMT+5)
- **Last Updated:** October 8, 2026
- **Version:** 3.0 — Red Team Edition 2026

> If this roadmap helps you learn, improve it, practice it legally, and pass the knowledge forward. Stay curious, stay ethical, and keep learning. 🟥🔐
