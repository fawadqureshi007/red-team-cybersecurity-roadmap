# 🟥 Red Team Cybersecurity Roadmap 2026
### From Fundamentals → Offensive Security → Red Team Tradecraft

> **A practical, research-driven roadmap for learning offensive security from the ground up.**
>
> The objective is not to collect tools or certificates. It is to understand systems well enough to reason about their attack surface, validate weaknesses in authorized environments, understand the defensive perspective, and communicate the result professionally.

**Author:** Fawad Qureshi  
**Focus:** Red Team / Offensive Security  
**Edition:** 2026  
**Approach:** Fundamentals → Practical Labs → Specialization → Professional Tradecraft

---

## 🧭 Before You Start

## 🔗 How to Use the Resources

Every phase now has a compact **Learn → Practice → Reference → Optional Book/Certification** layer. Do not collect links for the sake of collecting them. Pick one primary learning resource, one hands-on environment, and one reference source; finish the phase checkpoint before moving forward.

> **Rule:** official documentation teaches the system, labs build the skill, GitHub references speed up research, and books provide depth. Use all four deliberately.


There are thousands of cybersecurity resources online. The difficult part is usually not finding another course or another tool; it is knowing **what to learn first, what can wait, and how the pieces connect**.

This roadmap is organized around that problem.

The progression is intentional:

```text
Understand the technology
        ↓
Build and administer it
        ↓
Understand the security model
        ↓
Map the attack surface
        ↓
Validate weaknesses safely
        ↓
Understand privilege and identity
        ↓
Study enterprise environments
        ↓
Think in attack paths
        ↓
Understand detection
        ↓
Report professionally
        ↓
Specialize
```

The further down the roadmap you go, the less useful memorization becomes. At the advanced stages, judgment, troubleshooting, documentation, and understanding relationships matter much more than knowing another command.

---

# 📚 Contents

| # | Section | # | Section |
|---:|---|---:|---|
| 01 | [Roadmap Philosophy](#-roadmap-philosophy) | 19 | [AI Security](#-phase-17--ai-security) |
| 02 | [Who This Is For](#-who-this-is-for) | 20 | [Reporting](#-phase-18--reporting--professional-tradecraft) |
| 03 | [Legal Boundaries](#-legal--ethical-boundaries) | 21 | [Lab Architecture](#-practical-lab-architecture) |
| 04 | [Learning Model](#-the-learning-model) | 22 | [Platforms](#-recommended-learning-platforms) |
| 05 | [Phase 0: IT](#-phase-0--computer--it-foundations) | 23 | [Tool Categories](#-tool-categories) |
| 06 | [Phase 1: Networking](#-phase-1--networking) | 24 | [Certifications](#-certification-roadmap) |
| 07 | [Phase 2: Linux](#-phase-2--linux) | 25 | [Portfolio](#-portfolio-roadmap) |
| 08 | [Phase 3: Windows / AD](#-phase-3--windows--active-directory) | 26 | [Jobs](#-job-roles) |
| 09 | [Phase 4: Security](#-phase-4--security-fundamentals) | 27 | [Salaries](#-salary-guide--2026) |
| 10 | [Phase 5: Programming](#-phase-5--programming--scripting) | 28 | [6-Month Plan](#-6-month-roadmap) |
| 11 | [Phase 6: Recon](#-phase-6--reconnaissance--enumeration) | 29 | [12-Month Plan](#-12-month-roadmap) |
| 12 | [Phase 7: Web](#-phase-7--web-application-security) | 30 | [Weekly System](#-weekly-study-system) |
| 13 | [Phase 8: Vulnerability Research](#-phase-8--vulnerability-research) | 31 | [Progress](#-measuring-progress) |
| 14 | [Phase 9: Privilege](#-phase-9--privilege-escalation) | 32 | [Mistakes](#-common-mistakes) |
| 15 | [Phase 10: AD Security](#-phase-10--active-directory-security) | 33 | [Interview](#-interview-preparation) |
| 16 | [Phase 11: Internal Networks](#-phase-11--internal-network-security) | 34 | [Checklist](#-red-team-readiness-checklist) |
| 17 | [Phase 12: Cloud](#-phase-12--cloud-security) | 35 | [Resources](#-core-resources) |
| 18 | [Phase 13–16](#-phase-13--identity--access-security) | 36 | [FAQ / Final Advice](#-faq) |

---

# 🎯 Roadmap Philosophy

This roadmap follows five rules.

| Rule | Meaning |
|---|---|
| **Fundamentals first** | Networking, operating systems, identity and programming are not optional background knowledge. |
| **Practice every stage** | A topic should eventually become something you can reproduce in a legal lab. |
| **Understand the mechanism** | Learn why a technique works instead of memorizing a command. |
| **Think like both sides** | Understand what an attacker wants and what a defender can observe. |
| **Document the work** | Notes, evidence and reports turn isolated practice into professional skill. |

### The standard I recommend

> **Learn → Build → Enumerate → Analyze → Validate → Defend → Document**

If you cannot explain what happened, you probably do not understand it deeply enough yet.

---

# 👤 Who This Is For

This roadmap is designed for:

- complete beginners entering cybersecurity;
- IT or networking learners moving into security;
- aspiring penetration testers;
- red-team learners;
- SOC / blue-team analysts who want attacker perspective;
- security students building a structured study plan;
- practitioners who want to fill gaps in their fundamentals.

It is **not** designed as a "learn hacking in 30 days" checklist.

---

# ⚠️ Legal & Ethical Boundaries

Use these skills only against:

- systems you own;
- isolated personal labs;
- CTFs;
- intentionally vulnerable applications;
- authorized penetration-testing environments;
- bug-bounty targets that are explicitly in scope;
- systems for which you have clear written permission.

A professional assessment should have defined:

| Engagement Item | Examples |
|---|---|
| Scope | Domains, IP ranges, applications, identities |
| Time | Testing windows and maintenance periods |
| Methods | Allowed and prohibited techniques |
| Objectives | What the assessment is trying to demonstrate |
| Safety | Rate limits, production restrictions, stop conditions |
| Evidence | What may be collected and how it is stored |
| Communication | Primary and emergency contacts |

> **Authorization is part of the technical skill.**

---

# 🧠 The Learning Model

Don't treat the roadmap as a list where you simply tick boxes.

Use each phase at three levels:

### Level 1 — Understand

Can you explain the concept?

### Level 2 — Reproduce

Can you build or reproduce it in a controlled environment?

### Level 3 — Reason

Can you troubleshoot an unfamiliar example and explain the security implications?

The third level is where the real progress happens.

---

# 💻 Phase 0 — Computer & IT Foundations

Before testing a system, understand what the system is doing.

| Area | Learn | Target Understanding |
|---|---|---|
| Hardware | CPU · RAM · storage · peripherals | How hardware supports software execution |
| OS | Kernel · user space · processes · threads | How an OS manages programs |
| Filesystems | Paths · permissions · metadata · mounts | How data and access are organized |
| Processes | PID · parent/child · services · resources | How applications run |
| Virtualization | VM · snapshot · virtual network · NAT | How to build isolated labs |
| Administration | Users · groups · services · updates | How systems are normally operated |

### Foundation checkpoint

You should be able to explain:

```text
Program
  ↓
Process
  ↓
Memory + permissions
  ↓
Operating-system services
  ↓
Network / filesystem interaction
```

---

### 📚 Learn & Practice Resources

| Type | Resource | Why it belongs here |
|---|---|---|
| Learn | [Professor Messer A+](https://www.professormesser.com/) | Hardware, operating systems and troubleshooting fundamentals |
| Learn | [Linux Journey](https://linuxjourney.com/) | Beginner-friendly operating-system and command-line concepts |
| Practice | [OverTheWire](https://overthewire.org/wargames/) | Start applying command-line and system concepts through guided challenges |
| Lab | [VirtualBox](https://www.virtualbox.org/) | Build isolated virtual machines and snapshots for practice |
| Reference | [The Linux Command Line](https://nostarch.com/tlcl3) | Strong long-form reference for terminal and system fundamentals |

**Suggested checkpoint:** do not move on because you can follow a tutorial. Move on when you can build a small VM lab, explain processes/filesystems/permissions, and troubleshoot basic system problems yourself.


# 🌐 Phase 1 — Networking

Networking is one of the highest-value foundations in offensive security.

| Domain | Topics | What You Should Be Able to Explain |
|---|---|---|
| Addressing | IPv4 · IPv6 · CIDR · subnetting | How hosts and networks are addressed |
| Link layer | Ethernet · ARP | How local devices communicate |
| IP | Routing · gateways · ICMP | How traffic moves between networks |
| Transport | TCP · UDP · ports · sockets | How applications communicate |
| DNS | A · AAAA · CNAME · MX · TXT · NS | How names become infrastructure |
| DHCP | Leases · scopes · options | How hosts receive configuration |
| Web | HTTP · HTTPS · TLS | How browser/server communication works |
| Network design | NAT · VLANs · segmentation · firewalls | How environments are separated |
| Analysis | Packets · connections · captures | How to investigate traffic |

### Practice target

Build an isolated network containing:

```text
        Lab Network
             │
     ┌───────┼────────┐
     │       │        │
   Linux   Windows   Web App
```

Then identify the addressing, routes, services and traffic yourself.

### Useful resources

- Cisco Networking Academy
- Professor Messer Network+
- Beej's Guide to Network Programming

---

### 📚 Learn & Practice Resources

| Type | Resource | Best use |
|---|---|---|
| Learn | [Cisco Networking Academy](https://www.netacad.com/) | Networking fundamentals, packet flow and network configuration |
| Learn | [Professor Messer Network+](https://www.professormesser.com/network-plus/n10-009/n10-009-training-course/) | Structured Network+ study |
| Reference | [Beej's Guide to Network Programming](https://beej.us/guide/bgnet/) | Sockets and practical network programming |
| GitHub | [Awesome Networking](https://github.com/facyber/awesome-networking) | Curated networking references, tools and labs |
| Practice | [Wireshark](https://www.wireshark.org/docs/) | Learn by inspecting real packet captures |
| Book | [Computer Networking: A Top-Down Approach](https://www.pearson.com/en-us/subject-catalog/p/computer-networking-a-top-down-approach/P200000003302) | Deeper networking theory without losing the practical perspective |

**Lab idea:** capture DNS, TCP handshake, HTTP and TLS traffic in your own lab and explain each packet rather than memorizing port numbers.


# 🐧 Phase 2 — Linux

Linux should become a working environment, not just a machine where you run security tools.

| Area | Commands / Topics | Goal |
|---|---|---|
| Navigation | `pwd` · `ls` · `cd` | Understand paths and directories |
| Files | `cat` · `less` · `head` · `tail` | Inspect data efficiently |
| Search | `grep` · `find` | Locate files and information |
| Text | `sort` · `uniq` · `cut` · `awk` · `sed` | Process command output |
| Shell | Pipes · redirection · variables | Combine commands logically |
| Remote access | `ssh` | Understand remote administration |
| Web / transfer | `curl` · `wget` | Work with network resources |
| Permissions | Users · groups · ownership · mode bits | Understand access control |
| Processes | PID · services · signals | Understand running software |
| Networking | Interfaces · routes · sockets | Understand Linux networking |
| Administration | Packages · logs · services · scheduled tasks | Operate a Linux host |

### Linux mindset

For any file, process or service, ask:

> Who owns it?  
> Who can access it?  
> What runs it?  
> What does it communicate with?  
> What evidence does it leave?

---

### 📚 Learn & Practice Resources

| Type | Resource | Best use |
|---|---|---|
| Learn | [Linux Journey](https://linuxjourney.com/) | Linux concepts from beginner level |
| Practice | [OverTheWire Bandit](https://overthewire.org/wargames/bandit/) | Command line, permissions, files, SSH and problem solving |
| Reference | [Linux man-pages](https://man7.org/linux/man-pages/) | Primary reference for commands and system interfaces |
| GitHub | [Awesome Linux](https://github.com/aleksandar-todorovic/awesome-linux) | Curated Linux learning and tooling |
| Book | [The Linux Command Line](https://nostarch.com/tlcl3) | Shell, scripting and command-line fluency |
| Reference | [GTFOBins](https://gtfobins.github.io/) | Understand how Unix binaries can become security-relevant primitives in authorized labs |

**Practice rule:** learn commands in context. For example, understand what permissions, processes, pipes, services and sockets mean before turning them into pentesting checklists.


# 🪟 Phase 3 — Windows & Active Directory

Windows becomes especially important when you move into enterprise security.

## Windows foundations

| Area | Learn |
|---|---|
| Administration | Users · groups · services · scheduled tasks |
| PowerShell | Objects · pipeline · filtering · scripting |
| Security | Permissions · tokens · privileges |
| System | Registry · processes · drivers |
| Telemetry | Event Logs · auditing |
| Networking | SMB · DNS · remote administration concepts |

---

## 🏢 Active Directory Foundations

Learn the architecture before studying AD attack paths.

| Component | Understand |
|---|---|
| Domain | Central identity and administration boundary |
| Domain Controller | Core directory/authentication role |
| Users | Identity objects |
| Groups | Permission and access organization |
| OU | Administrative organization |
| GPO | Centralized configuration |
| LDAP | Directory communication concepts |
| Kerberos | Enterprise authentication concepts |
| NTLM | Legacy authentication concepts |
| DNS | AD dependency and name resolution |
| Trusts | Relationships between domains/forests |
| ACLs | Permissions and object access |
| Service accounts | Non-human identities |

### Core idea

> **AD security is largely identity + permissions + trust relationships.**

---

### 📚 Learn & Practice Resources

| Type | Resource | Best use |
|---|---|---|
| Learn | [Microsoft Learn — Windows](https://learn.microsoft.com/windows/) | Windows administration and internals foundations |
| Learn | [Microsoft Learn — Active Directory Domain Services](https://learn.microsoft.com/windows-server/identity/ad-ds/) | Domain, authentication, policy and directory concepts |
| Lab | [GOAD](https://github.com/Orange-Cyberdefense/GOAD) | Vulnerable Active Directory environment for authorized practice |
| GitHub | [Commando VM](https://github.com/mandiant/commando-vm) | Windows-based offensive-security lab/tool environment |
| Reference | [AD Security](https://adsecurity.org/) | Active Directory security research and concepts |
| Book | [Windows Internals / Sysinternals](https://learn.microsoft.com/en-us/sysinternals/resources/windows-internals) | Use Sysinternals plus Windows internals material to understand what Windows is actually doing |

**Lab goal:** build or use an isolated domain and learn to explain users, groups, OUs, GPOs, Kerberos, NTLM, LDAP, DNS and ACLs before studying attack paths.


# 🔐 Phase 4 — Security Fundamentals

| Area | Core Concepts |
|---|---|
| CIA | Confidentiality · Integrity · Availability |
| Identity | Authentication · Authorization · Accounting |
| Risk | Threat · vulnerability · likelihood · impact |
| Crypto | Hashing · encryption · signatures · certificates · TLS |
| Vulnerabilities | Injection · access control · disclosure · misconfiguration |
| Security controls | Preventive · detective · corrective |
| Monitoring | Logging · alerting · telemetry |
| Response | Identification · containment · eradication · recovery |

### Frameworks to understand

| Framework | Why Learn It |
|---|---|
| NIST CSF | Organizing cybersecurity risk |
| CIS Controls | Prioritized security controls |
| MITRE ATT&CK | Adversary behavior and techniques |
| MITRE D3FEND | Defensive countermeasures |
| MITRE ATLAS | AI threat behavior |
| OWASP | Application security |

---

### 📚 Learn & Practice Resources

| Type | Resource | Best use |
|---|---|---|
| Framework | [NIST Cybersecurity Framework](https://www.nist.gov/cyberframework) | Understand security outcomes and risk thinking |
| Framework | [CIS Controls](https://www.cisecurity.org/controls) | Practical defensive controls and priorities |
| Threat model | [MITRE ATT&CK](https://attack.mitre.org/) | Map attacker behavior to techniques and defensive visibility |
| Learn | [ISC2 Certified in Cybersecurity](https://www.isc2.org/certifications/cc) | Entry-level security foundation and certification path |
| Learn | [CompTIA Security+](https://www.comptia.org/certifications/security) | Broad security fundamentals and terminology |
| Practice | [picoCTF](https://picoctf.org/) | Beginner-friendly security problem solving |

**Certification note:** CC is designed for newcomers with no work experience; Security+ is a broader baseline. Neither replaces hands-on labs.


# 🐍 Phase 5 — Programming & Scripting

You do not need to become a software engineer.

You do need to read, modify and write enough code to automate work and understand applications.

| Language | Priority | Security Use |
|---|---:|---|
| Python | ⭐⭐⭐⭐⭐ | Automation · APIs · analysis · tooling |
| Bash | ⭐⭐⭐⭐ | Linux automation |
| PowerShell | ⭐⭐⭐⭐⭐ | Windows administration and automation |
| SQL | ⭐⭐⭐⭐ | Databases and application security |
| JavaScript | ⭐⭐⭐⭐ | Web applications and browser behavior |
| C/C++ | ⭐⭐⭐ | Memory and binary fundamentals |

### Python progression

```text
Syntax
 → Functions
 → Files
 → JSON
 → Exceptions
 → HTTP
 → Sockets
 → Regex
 → APIs
 → Automation
```

The objective is not to collect scripts. It is to understand and build them.

---

### 📚 Learn & Practice Resources

| Type | Resource | Best use |
|---|---|---|
| Learn | [Python Official Tutorial](https://docs.python.org/3/tutorial/) | Python syntax, data structures and standard library |
| Learn | [Automate the Boring Stuff](https://automatetheboringstuff.com/) | Practical Python automation |
| Practice | [pwn.college](https://pwn.college/) | Hands-on programming, exploitation and systems challenges |
| GitHub | [Awesome Python](https://github.com/vinta/awesome-python) | Find useful Python libraries and learning references |
| Book | [Black Hat Python](https://nostarch.com/black-hat-python2e) | Security-oriented Python projects and automation |
| Learn | [Bash Reference Manual](https://www.gnu.org/software/bash/manual/) | Shell scripting and automation |

**Project target:** write small utilities that parse scan output, query an API, process logs, manipulate files and automate repetitive lab work.


# 🔎 Phase 6 — Reconnaissance & Enumeration

Recon is the process of building an accurate picture of an authorized environment.

| Stage | Questions |
|---|---|
| Discovery | What assets exist? |
| Identification | What are these assets? |
| Services | What is exposed? |
| Technology | What software/frameworks are involved? |
| Configuration | How are they configured? |
| Identity | What authentication exists? |
| Relationships | How do systems trust each other? |
| Validation | Which observations deserve deeper testing? |

### Keep structured notes

```text
Asset
├── Hostname
├── Address
├── Service
├── Technology
├── Version
├── Authentication
├── Interesting behavior
├── Evidence
└── Follow-up question
```

> **Enumeration is where curiosity becomes methodology.**

---

### 📚 Learn & Practice Resources

| Type | Resource | Best use |
|---|---|---|
| Methodology | [OWASP Web Security Testing Guide](https://owasp.org/www-project-web-security-testing-guide/) | Structured web reconnaissance/testing methodology |
| Reference | [Nmap Documentation](https://nmap.org/book/) | Service discovery and network enumeration theory |
| GitHub | [ProjectDiscovery](https://github.com/projectdiscovery) | Modern open-source recon and asset-discovery tooling |
| GitHub | [reconftw](https://github.com/six2dez/reconftw) | Study how recon workflows are assembled; use only on authorized targets |
| Practice | [Hack The Box](https://www.hackthebox.com/) | Enumeration against intentionally vulnerable targets |
| Practice | [TryHackMe](https://tryhackme.com/) | Guided recon and enumeration learning paths |

**Note:** recon is not “run 20 tools.” Build an asset inventory, record evidence and explain why each next step follows from the previous observation.


# 🌍 Phase 7 — Web Application Security

Web security deserves serious attention because modern organizations expose large amounts of functionality through web applications and APIs.

## Understand the stack

```text
Browser
   ↓
DNS
   ↓
TLS
   ↓
Web Server
   ↓
Application
   ↓
API / Database / Services
```

| Area | Learn |
|---|---|
| HTTP | Methods · headers · status codes · content types |
| Sessions | Cookies · tokens · session lifecycle |
| Authentication | Login · recovery · MFA concepts |
| Authorization | Roles · object ownership · access control |
| Input | Validation · encoding · interpretation |
| APIs | Endpoints · authentication · authorization |
| Browser | DOM · JavaScript · same-origin concepts |
| Architecture | Reverse proxies · application servers · databases |

## OWASP-focused study

Study:

- broken access control;
- authentication failures;
- injection;
- cryptographic failures;
- security misconfiguration;
- vulnerable components;
- identification and authentication weaknesses;
- software/data integrity failures;
- logging and monitoring weaknesses;
- SSRF;
- insecure design.

### The important question

> **Where does user-controlled data go, and what interprets it next?**

---

### 📚 Learn & Practice Resources

| Type | Resource | Best use |
|---|---|---|
| Learn + Labs | [PortSwigger Web Security Academy](https://portswigger.net/web-security) | One of the strongest free hands-on web-security learning paths |
| Standard | [OWASP Top 10](https://owasp.org/www-project-top-ten/) | Common web application risk categories |
| Methodology | [OWASP WSTG](https://owasp.org/www-project-web-security-testing-guide/) | Detailed testing methodology |
| Lab | [OWASP Juice Shop](https://github.com/juice-shop/juice-shop) | Intentionally vulnerable modern web application |
| GitHub | [PayloadsAllTheThings](https://github.com/swisskyrepo/PayloadsAllTheThings) | Reference for web-security testing ideas and payload patterns |
| API Lab | [vAPI](https://github.com/roottusk/vapi) | Practice OWASP API security scenarios locally |
| Book | [The Web Application Hacker's Handbook](https://www.oreilly.com/library/view/the-web-application/9781118026470/) | Classic reference; pair it with current PortSwigger Academy material |

**Recommended order:** HTTP → sessions/auth → access control → injection → XSS → SSRF → file handling → APIs → business logic.


# 🧪 Phase 8 — Vulnerability Research

Don't jump directly from "I found a version" to "I found an exploit."

Use:

```text
Observation
    ↓
Hypothesis
    ↓
Reproduction
    ↓
Validation
    ↓
Impact
    ↓
Evidence
    ↓
Remediation
```

| Skill | Learn |
|---|---|
| CVE literacy | Affected versions · prerequisites · severity |
| Root cause | Why the weakness exists |
| Reproduction | Controlled validation |
| False positives | Why scanners can be wrong |
| Impact | What the weakness actually enables |
| Remediation | How the condition should be removed |

### Important distinction

> **A CVE does not automatically mean a particular target is exploitable.**

Always verify the actual conditions.

---

### 📚 Learn & Practice Resources

| Type | Resource | Best use |
|---|---|---|
| Vulnerability data | [NVD](https://nvd.nist.gov/) | CVEs, affected products and vulnerability metadata |
| Vulnerability data | [CVE.org](https://www.cve.org/) | Primary CVE ecosystem and identifiers |
| Research | [Google Project Zero](https://googleprojectzero.blogspot.com/) | Read high-quality vulnerability research and root-cause analysis |
| Practice | [pwn.college](https://pwn.college/) | Vulnerability and exploitation fundamentals |
| GitHub | [OSS-Fuzz](https://github.com/google/oss-fuzz) | Learn how large-scale fuzzing finds software bugs |
| Reference | [Exploit-DB](https://www.exploit-db.com/) | Study public exploit history and research patterns; validate safely |

**Research habit:** reproduce in a controlled environment, identify root cause, document impact and determine the smallest reliable fix.


# ⬆️ Phase 9 — Privilege Escalation

Privilege escalation is fundamentally an access-control problem.

### Linux

| Area | Study |
|---|---|
| Permissions | Files · directories · ownership |
| Sudo | Delegated administrative access |
| Services | Service identity and configuration |
| Scheduled tasks | Automated execution |
| Environment | Variables and execution context |
| Processes | Ownership and privileges |
| Credentials | Where sensitive authentication material may reside |

### Windows

| Area | Study |
|---|---|
| Services | Service accounts and permissions |
| Scheduled tasks | Execution context |
| Tokens | Identity and privilege concepts |
| Groups | Local membership |
| Privileges | Windows security privileges |
| Registry | Permissions and configuration |
| Credentials | Secure credential-handling concepts |

The central question:

> **What can this identity access that it should not be able to access?**

---

### 📚 Learn & Practice Resources

| Type | Resource | Best use |
|---|---|---|
| Reference | [GTFOBins](https://gtfobins.github.io/) | Unix/Linux privilege and execution primitives |
| Reference | [LOLBAS](https://lolbas-project.github.io/) | Windows binaries that can have security-relevant uses |
| Learn | [HackTricks](https://book.hacktricks.wiki/) | Broad pentesting and privilege-escalation reference |
| Practice | [Hack The Box](https://www.hackthebox.com/) | Vulnerable machines requiring enumeration and escalation |
| Practice | [TryHackMe](https://tryhackme.com/) | Guided Linux/Windows privilege-escalation rooms |
| GitHub | [PayloadsAllTheThings](https://github.com/swisskyrepo/PayloadsAllTheThings) | Cross-platform pentesting reference |

**Mindset:** ask “what security boundary prevents this action?” rather than memorizing a list of tricks.


# 🏢 Phase 10 — Active Directory Security

Once the AD architecture makes sense, start thinking in attack paths.

| Area | Understand |
|---|---|
| Kerberos | Authentication and ticket concepts |
| LDAP | Directory information |
| ACLs | Object permissions |
| Groups | Privilege relationships |
| GPO | Centralized configuration |
| Delegation | Identity/service relationships |
| Service accounts | Non-human identity risk |
| Trusts | Cross-domain relationships |
| Sessions | Where privileged identities operate |

### Attack-path thinking

```text
Identity
   ↓
Group / Permission
   ↓
Resource
   ↓
New Access
   ↓
Another Identity
   ↓
Higher Privilege
```

The goal is to understand **why the path exists**, not memorize a list of tricks.

---

### 📚 Learn & Practice Resources

| Type | Resource | Best use |
|---|---|---|
| Lab | [GOAD](https://github.com/Orange-Cyberdefense/GOAD) | Purpose-built AD pentesting lab |
| Reference | [BloodHound Community Edition](https://github.com/SpecterOps/BloodHound) | Understand and visualize identity relationships and attack paths |
| Reference | [AD Security](https://adsecurity.org/) | Deep AD security research |
| Reference | [InternalAllTheThings](https://github.com/swisskyrepo/InternalAllTheThings) | Internal/AD pentesting reference material |
| Learn | [Microsoft AD DS documentation](https://learn.microsoft.com/windows-server/identity/ad-ds/) | Understand the legitimate architecture first |
| Practice | [TryHackMe AD content](https://tryhackme.com/) | Guided identity and domain labs |

**Certification direction:** build real AD lab ability before considering advanced offensive certifications such as OSCP+/OSEP/CRTO.


# 🔀 Phase 11 — Internal Network Security

Study how enterprise networks are divided and where trust boundaries exist.

| Area | Learn |
|---|---|
| Segmentation | VLANs · security zones |
| Routing | Internal routes and gateways |
| Firewalls | Filtering between zones |
| Proxies | Controlled network access |
| Identity | Workstation/server relationships |
| Administration | Privileged management paths |
| Services | Shared enterprise infrastructure |
| Trust | What one system assumes about another |

### Defensive question

> If one workstation were compromised, what should stop the attacker from reaching the next important system?

That question naturally connects red-team testing with architecture and defense.

---

### 📚 Learn & Practice Resources

| Type | Resource | Best use |
|---|---|---|
| Practice | [Hack The Box](https://www.hackthebox.com/) | Internal network and multi-host practice |
| Practice | [Proving Grounds](https://www.offsec.com/labs/proving-grounds/) | Structured offensive-security labs |
| Reference | [MITRE ATT&CK](https://attack.mitre.org/) | Map internal techniques to attacker behavior |
| GitHub | [InternalAllTheThings](https://github.com/swisskyrepo/InternalAllTheThings) | Internal pentesting and AD reference |
| Learn | [Wireshark Documentation](https://www.wireshark.org/docs/) | Analyze internal traffic and protocols |
| Framework | [CIS Controls](https://www.cisecurity.org/controls) | Understand segmentation, hardening and monitoring from the defensive side |

**Lab target:** understand how a foothold can become an identity, network or application path without treating lateral movement as a bag of commands.


# ☁️ Phase 12 — Cloud Security

Choose at least one major platform:

- AWS
- Microsoft Azure
- Google Cloud

| Area | Learn |
|---|---|
| Organization | Accounts · subscriptions · projects |
| Compute | VMs · containers · serverless |
| Networking | VPC/VNet · routing · security groups |
| Storage | Buckets · object access |
| IAM | Users · roles · policies |
| Secrets | Keys · tokens · secret stores |
| Logging | Audit trails · activity logs |
| Workloads | Service identities and permissions |

### Cloud security is heavily identity-driven.

Ask:

> Who can access this resource, with which identity, under which conditions, and what evidence is logged?

---

### 📚 Learn & Practice Resources

| Type | Resource | Best use |
|---|---|---|
| AWS | [AWS Security Documentation](https://docs.aws.amazon.com/security/) | IAM, logging, network and service security |
| Azure | [Microsoft Cloud Security](https://learn.microsoft.com/security/) | Azure identity, security and architecture |
| Framework | [MITRE ATT&CK Cloud](https://attack.mitre.org/matrices/enterprise/cloud/) | Cloud attacker behavior and techniques |
| Lab | [AWSGoat](https://github.com/ine-labs/AWSGoat) | Deliberately vulnerable AWS environment |
| Lab | [CloudGoat](https://github.com/RhinoSecurityLabs/cloudgoat) | Vulnerable-by-design AWS scenarios |
| GitHub | [Cloud Security Alliance](https://github.com/CloudSecurityAlliance) | Cloud-security standards and projects |

**Important:** cloud labs can create real costs. Use dedicated test accounts, least privilege, budgets and teardown procedures. AWSGoat itself notes that charges can apply outside free-tier conditions.


# 🪪 Phase 13 — Identity & Access Security

Identity connects traditional infrastructure, cloud and applications.

| Topic | Understand |
|---|---|
| MFA | Additional authentication factors |
| SSO | Centralized authentication |
| OAuth | Delegated authorization |
| OIDC | Identity layer over OAuth |
| SAML | Enterprise federation concepts |
| RBAC | Role-based permissions |
| ABAC | Attribute-based decisions |
| Service accounts | Non-human identities |
| Secrets | Keys, tokens and credentials |
| Machine identity | Workloads and services |

### 2026 focus

Pay particular attention to:

- machine identities;
- API keys;
- CI/CD credentials;
- cloud roles;
- service accounts;
- AI-agent identities.

---

### 📚 Learn & Practice Resources

| Type | Resource | Best use |
|---|---|---|
| Framework | [NIST Digital Identity Guidelines](https://pages.nist.gov/800-63-4/) | Authentication and identity assurance concepts |
| Learn | [Microsoft Entra ID documentation](https://learn.microsoft.com/entra/) | Modern enterprise identity and access management |
| Learn | [OAuth 2.0](https://oauth.net/2/) | Authorization flows and terminology |
| Learn | [OpenID Connect](https://openid.net/developers/how-connect-works/) | Identity layer built on OAuth 2.0 |
| Practice | [PortSwigger Authentication Labs](https://portswigger.net/web-security/authentication) | Apply authentication/session concepts |
| Reference | [OWASP ASVS](https://owasp.org/www-project-application-security-verification-standard/) | Application-level identity and access-control requirements |

**Core question:** who is the subject, what is it allowed to do, where is that decision enforced, and what happens when the identity boundary fails?


# 🎯 Phase 14 — Adversary Simulation & Red Team Operations

Red teaming is broader than finding vulnerabilities.

A mature exercise asks whether an organization can:

- prevent;
- detect;
- investigate;
- respond;
- recover;
- and improve.

## Engagement lifecycle

| Stage | Focus |
|---|---|
| Planning | Objectives and scope |
| Rules of Engagement | Safety and authorization |
| Recon | Build the environment picture |
| Initial Access Simulation | Test an approved entry path |
| Access Analysis | Understand permissions |
| Objective | Demonstrate agreed impact |
| Detection | Observe defensive visibility |
| Cleanup | Return the environment to agreed state |
| Reporting | Explain findings and risk |
| Debrief | Improve defenses |

### The operator mindset

Don't ask only:

> "Can this work?"

Also ask:

> "Why does it work, what evidence would it produce, what control should stop it, and how would I explain the result?"

---

### 📚 Learn & Practice Resources

| Type | Resource | Best use |
|---|---|---|
| Framework | [MITRE ATT&CK](https://attack.mitre.org/) | Adversary behaviors and technique mapping |
| Methodology | [MITRE Adversary Emulation Plans](https://github.com/center-for-threat-informed-defense/adversary_emulation_library) | Study realistic adversary behaviors in controlled environments |
| Framework | [Atomic Red Team](https://github.com/redcanaryco/atomic-red-team) | Small, testable security-validation techniques |
| Platform | [CALDERA](https://github.com/mitre/caldera) | Automated adversary emulation in controlled environments |
| Lab | [Prelude Operator](https://www.prelude.org/) | Adversary simulation and detection validation |
| Reference | [Red Team Field Manual](https://github.com/leostat/rtfm) | Compact field reference; use as a supplement, not a curriculum |

**Professional requirement:** learn rules of engagement, authorization, evidence handling, safety controls, objectives and reporting before attempting realistic simulations.


# 🕵️ Phase 15 — OPSEC & Detection Awareness

OPSEC in professional red teaming is not simply "hide from defenders."

It is about understanding exposure, constraints and the telemetry generated by activity.

| Defensive Visibility | Study |
|---|---|
| Endpoint | Processes · files · registry · security events |
| Network | Connections · DNS · proxy · traffic |
| Identity | Authentication · privilege events |
| Cloud | Audit logs · API activity |
| SIEM | Correlation and alerting |
| EDR | Endpoint detection and investigation |
| Detection engineering | Turning telemetry into useful detections |

For every technique, ask:

```text
What happens?
        ↓
What telemetry exists?
        ↓
What might trigger an alert?
        ↓
What should the defender investigate?
```

---

### 📚 Learn & Practice Resources

| Type | Resource | Best use |
|---|---|---|
| Detection | [MITRE ATT&CK](https://attack.mitre.org/) | Understand what defenders can observe |
| Detection | [Sigma](https://sigmahq.io/) | Study portable detection logic |
| Detection | [Sysmon](https://learn.microsoft.com/sysinternals/downloads/sysmon) | Generate useful Windows telemetry in a lab |
| Lab | [Blue Team Labs Online](https://blueteamlabs.online/) | Use blue-team labs to understand telemetry and investigation |
| Framework | [NIST CSF](https://www.nist.gov/cyberframework) | Connect offensive findings to defensive outcomes |
| Learn | [MITRE ATT&CK Data Sources](https://attack.mitre.org/datasources/) | Understand what telemetry can support detection |

**Important distinction:** OPSEC in this roadmap means controlled, engagement-aware behavior and understanding defensive visibility—not instructions for evading law enforcement or hiding unauthorized activity.


# 🦠 Phase 16 — Malware & Reverse Engineering

This is an advanced specialization and should come after strong OS and programming fundamentals.

| Area | Learn |
|---|---|
| Static analysis | Files · strings · imports · structure |
| Dynamic analysis | Runtime behavior |
| Debugging | Execution and memory |
| Binary formats | PE / ELF concepts |
| Assembly | Basic instruction-level understanding |
| Processes | Memory and execution |
| Network behavior | Communication patterns |

Useful tools for isolated research environments include:

- Ghidra
- x64dbg
- Wireshark
- Procmon
- Autoruns
- sandboxing platforms

Only analyze unknown or malicious samples in properly isolated environments.

---

### 📚 Learn & Practice Resources

| Type | Resource | Best use |
|---|---|---|
| Tool | [Ghidra](https://github.com/NationalSecurityAgency/ghidra) | Static analysis, disassembly and reverse engineering |
| Tool | [x64dbg](https://x64dbg.com/) | Windows debugging |
| Reference | [Windows Sysinternals](https://learn.microsoft.com/sysinternals/) | Process, filesystem and Windows behavior analysis |
| Tool | [Volatility 3](https://github.com/volatilityfoundation/volatility3) | Memory analysis and forensic investigation |
| Practice | [picoCTF](https://picoctf.org/) | Beginner-friendly reverse-engineering challenges |
| Book | [Practical Malware Analysis](https://nostarch.com/malware) | Classic malware-analysis foundation; use in an isolated lab |

**Safety rule:** never execute unknown samples on your normal machine. Use isolated VMs, controlled networking, snapshots and appropriate analysis procedures.


# 🤖 Phase 17 — AI Security

AI security is now part of the modern attack surface.

| Area | Study |
|---|---|
| Prompt injection | Manipulating model instructions |
| Data exposure | Sensitive information reaching models |
| Tool abuse | AI systems interacting with external tools |
| Agent security | Identity and permissions of AI agents |
| Supply chain | Models, datasets and dependencies |
| Data poisoning | Manipulation of training/input data |
| Model extraction | Unauthorized recovery of model behavior |
| Social engineering | AI-assisted impersonation and persuasion |

### Frameworks

- OWASP Top 10 for LLM Applications
- MITRE ATLAS
- NIST AI Risk Management Framework

A particularly important modern question:

> **What can an AI agent do if its identity, tools or permissions are abused?**

---

### 📚 Learn & Practice Resources

| Type | Resource | Best use |
|---|---|---|
| Standard | [OWASP GenAI Security Project](https://genai.owasp.org/) | Current LLM/GenAI security risks and guidance |
| Framework | [MITRE ATLAS](https://atlas.mitre.org/) | Adversarial threats against AI-enabled systems |
| Framework | [NIST AI RMF](https://www.nist.gov/itl/ai-risk-management-framework) | AI risk-management concepts |
| Practice | [OWASP Web Security Academy](https://portswigger.net/web-security) | Keep web/API security fundamentals strong while learning AI security |
| GitHub | [OWASP GenAI Security Project](https://github.com/OWASP/www-project-top-10-for-large-language-model-applications) | Community-maintained LLM security material |
| Research | [Google DeepMind Security](https://deepmind.google/discover/blog/) | Follow current AI safety/security research |

**Study order:** application architecture → model interaction → prompt/data boundaries → tool permissions → agent identity → logging/evaluation → adversarial testing.


# 📝 Phase 18 — Reporting & Professional Tradecraft

A technically correct finding is not enough.

A professional report should allow a technical team and a decision-maker to understand the same issue from different perspectives.

| Report Section | Purpose |
|---|---|
| Title | State the problem clearly |
| Severity | Prioritize the issue |
| Affected Asset | Define scope |
| Description | Explain the condition |
| Evidence | Prove the observation |
| Impact | Explain business/security consequences |
| Reproduction | Allow authorized validation |
| Remediation | Give a practical fix |
| References | Support further investigation |

### Finding template

```text
Finding:
Severity:
Affected Asset:
Description:
Evidence:
Impact:
Recommendation:
Validation / Retest:
References:
```

### Good reporting is a security skill.

If you cannot explain the issue clearly, the technical work is incomplete.

---

### 📚 Learn & Practice Resources

| Type | Resource | Best use |
|---|---|---|
| Methodology | [OWASP WSTG](https://owasp.org/www-project-web-security-testing-guide/) | Learn how professional technical testing is structured |
| Framework | [PTES](http://www.pentest-standard.org/) | Penetration-testing methodology and engagement structure |
| Framework | [NIST SP 800-115](https://csrc.nist.gov/pubs/sp/800/115/final) | Technical security-testing guidance |
| Reference | [MITRE ATT&CK](https://attack.mitre.org/) | Communicate techniques using a common vocabulary |
| Practice | [Hack The Box](https://www.hackthebox.com/) | Produce your own technical notes and reports from lab work |
| Book | [The Practice of Network Security Monitoring](https://nostarch.com/nsm) | Strengthen the defensive/reporting perspective |

**Portfolio rule:** publish sanitized, legal lab reports—not client data, secrets, credentials or unauthorized findings.


# 🧪 Practical Lab Architecture

Start small and grow the environment.

## Level 1

```text
Host
 ├── Linux VM
 ├── Windows VM
 └── Vulnerable Web Application
```

## Level 2

```text
             Isolated Lab Network
                    │
          ┌─────────┼─────────┐
          │         │         │
       Linux     Windows    Web App
                    │
              Windows Server
```

## Level 3

```text
                 Domain Controller
                        │
            ┌───────────┼───────────┐
            │           │           │
       Workstation    Server     Admin VM
            │           │
            └──────┬────┘
                   │
             Security Lab
```

The objective is not to build the largest lab.

The objective is to create an environment where you can **observe, break, troubleshoot, restore and document**.

---

# 🌐 Recommended Learning Platforms

| Platform | Best For |
|---|---|
| **TryHackMe** | Guided beginner-to-intermediate learning |
| **Hack The Box** | Practical labs and independent problem solving |
| **PortSwigger Web Security Academy** | Deep web-security practice |
| **OverTheWire** | Linux and command-line fundamentals |
| **OWASP Juice Shop** | Web application security |
| **VulnHub** | Vulnerable local VMs |
| **Microsoft Learn** | Windows, Azure and security fundamentals |

---

# 🧰 Tool Categories

Don't install everything at once.

Learn the category first.

| Category | Examples | Purpose |
|---|---|---|
| Network analysis | Wireshark · tcpdump | Inspect traffic |
| Service discovery | Nmap | Understand exposed services |
| Web testing | Burp Suite | Analyze web applications |
| Browser analysis | Developer Tools | Inspect client-side behavior |
| AD analysis | Directory / graph analysis tools | Understand identity relationships |
| Reverse engineering | Ghidra · x64dbg | Analyze binaries |
| System analysis | Procmon · Autoruns | Understand Windows behavior |
| Documentation | Markdown · diagrams | Preserve evidence and findings |

> **Tool knowledge is useful. Tool dependency is not.**

---

# 📜 Certification Roadmap

Certifications should validate skills you are already building. They are not substitutes for labs, projects or fundamentals. Current official references are linked below.

| Stage | Certification | Best fit | When to consider it | Official
|---|---|---|---|---|
| Beginner | ISC2 CC | First cybersecurity credential | After Phase 4 fundamentals | [ISC2 CC](https://www.isc2.org/certifications/cc) |
| Beginner | CompTIA Network+ | Networking foundation | Around Phase 1–4 if you want a structured baseline | [Network+](https://www.comptia.org/certifications/network) |
| Beginner / Core | CompTIA Security+ | Broad security foundation | After networking + security fundamentals | [Security+](https://www.comptia.org/certifications/security) |
| Entry offensive | eJPT | First practical pentesting milestone | After networking, Linux, Windows and basic web testing | [eJPT](https://security.ine.com/certifications/ejpt-certification/) |
| Practical pentest | PNPT | Practical pentesting/reporting | After solid hands-on fundamentals | [TCM Certifications](https://certifications.tcm-sec.com/) |
| Advanced pentest | OSCP+ | Serious hands-on penetration testing | After substantial lab experience | [OSCP+](https://help.offsec.com/hc/en-us/articles/360040165632-OSCP-Exam-Guide) |
| Advanced offensive | OSEP | Advanced exploitation and adversary simulation | After strong OSCP-level skills | [OffSec](https://www.offsec.com/courses/pen-300/) |
| Red team | CRTO | Command-and-control/red-team tradecraft | After strong AD, Windows and network skills | [Zero-Point Security](https://training.zeropointsecurity.co.uk/) |
| Web security | OSWA / OSWE | Web application specialization | After serious PortSwigger/OWASP practice | [OffSec Web](https://www.offsec.com/courses/) |
| Cloud | Cloud-specific certs | AWS/Azure/GCP security | After real cloud fundamentals and labs | [AWS Security](https://aws.amazon.com/certification/); [Microsoft Security](https://learn.microsoft.com/credentials/) |

### 🎯 Recommended Red-Team Sequence

```text
Networking + Linux + Windows
          ↓
Security fundamentals
          ↓
Web + enumeration + scripting
          ↓
Hands-on labs / CTFs
          ↓
eJPT / PNPT (optional milestone)
          ↓
Active Directory + internal networks
          ↓
Serious lab portfolio
          ↓
OSCP+
          ↓
OSEP / CRTO / OSWA / OSWE / cloud specialization
```

**Do not buy every certification.** Pick credentials that match the role you actually want. OffSec currently lists PEN-200/OSCP, WEB-200/OSWA, WEB-300/OSWE, PEN-300 and other specialist paths; OSCP+ can also be purchased as a standalone exam if you already have the required skill level.

# 🏆 Portfolio Roadmap

A strong portfolio should show **how you think**, not just what tools you used.

| Stage | Project | Demonstrates |
|---|---|---|
| Beginner | Network lab | Networking fundamentals |
| Beginner | Linux hardening | Administration + security |
| Beginner | Windows lab | Windows fundamentals |
| Intermediate | Web assessment | Application security |
| Intermediate | AD lab | Identity + enterprise security |
| Intermediate | Detection lab | Offensive + defensive thinking |
| Advanced | Cloud IAM review | Cloud security |
| Advanced | Adversary simulation lab | Red-team methodology |
| Advanced | Research report | Technical investigation |

### Each project should contain

```text
Objective
Environment
Methodology
Observations
Evidence
Findings
Impact
Remediation
Lessons Learned
```

Never publish:

- client information;
- credentials;
- secrets;
- private infrastructure;
- personal information;
- confidential reports.

---

# 💼 Job Roles

## Entry

| Role | Useful Foundations |
|---|---|
| SOC Analyst | Security + networking + logs |
| Junior Security Analyst | Security + systems |
| Security Intern | Fundamentals + labs |
| Junior Pentester | Networking + Linux + web |
| Vulnerability Analyst | Vulnerability management + systems |

## Intermediate

| Role | Useful Skills |
|---|---|
| Penetration Tester | Web + network + privilege |
| Security Engineer | Systems + security architecture |
| AppSec Engineer | Web + code + SDLC |
| Cloud Security Engineer | Cloud + IAM |
| Detection Engineer | Telemetry + detection |

## Advanced

| Role | Useful Skills |
|---|---|
| Red Team Operator | AD + identity + adversary simulation |
| Senior Pentester | Broad offensive depth |
| Security Researcher | Programming + vulnerability research |
| Red Team Lead | Technical depth + planning + reporting |
| Security Architect | Broad systems + security design |

---

# 💰 Salary Guide — 2026

> **These are broad market-oriented planning ranges, not guarantees.** Actual compensation depends on city, experience, employer, specialization, clearance, bonuses, benefits and local market conditions.

| Country | Entry Cyber/SOC | Junior Pentest | Security Engineer / Pentest | Experienced Red Team |
|---|---:|---:|---:|---:|
| 🇵🇰 Pakistan | PKR 50K–120K/mo | PKR 80K–180K/mo | PKR 120K–300K/mo | PKR 250K–600K+ /mo |
| 🇮🇳 India | ₹3–8 LPA | ₹4–10 LPA | ₹6–15 LPA | ₹10–25+ LPA |
| 🇺🇸 USA | US$70K–100K | US$80K–120K | US$100K–150K | US$140K–200K+ |
| 🇨🇦 Canada | C$60K–85K | C$70K–100K | C$90K–125K | C$115K–160K+ |
| 🇦🇺 Australia | A$75K–105K | A$70K–95K | A$95K–130K | A$140K–190K+ |

### Australia senior progression

Australian salary guides can show higher ranges at senior/principal level:

| Role | Approx. 2026 Range |
|---|---:|
| Junior Penetration Tester | A$70K–95K |
| Penetration Tester | A$95K–130K |
| Senior Penetration Tester | A$140K–160K |
| Principal Penetration Tester | A$155K–190K |

Salary data should always be treated as a market snapshot. A certification alone does not determine compensation.

---

# 📅 6-Month Roadmap

| Month | Focus | Practical Deliverable |
|---:|---|---|
| 1 | Networking + Linux + Windows | Build an isolated lab |
| 2 | Security fundamentals + scripting | Security notes + first report |
| 3 | HTTP + web security | Web-security lab report |
| 4 | Recon + enumeration + privilege concepts | Multiple documented labs |
| 5 | AD + cloud + identity | AD/cloud lab documentation |
| 6 | Red-team methodology + portfolio | Portfolio + certification preparation |

---

# 🗓️ 12-Month Roadmap

| Quarter | Focus | Goal |
|---|---|---|
| Q1 | Networking · Linux · Windows · Python | Strong technical foundation |
| Q2 | Web · Recon · Vulnerability · Privilege | Offensive fundamentals |
| Q3 | AD · Cloud · IAM · specialization | Domain depth |
| Q4 | Red Team · Detection · Reporting · Portfolio | Professional readiness |

---

# ⏱️ Weekly Study System

## 1 Hour / Day

| Time | Activity |
|---:|---|
| 20 min | Theory |
| 30 min | Lab |
| 10 min | Notes |

## 2 Hours / Day

| Time | Activity |
|---:|---|
| 30 min | Theory |
| 70 min | Practical |
| 20 min | Documentation |

## 4 Hours / Day

| Time | Activity |
|---:|---|
| 45 min | Theory |
| 2 hr | Practical lab |
| 45 min | Research |
| 30 min | Documentation |

The exact schedule matters less than maintaining the cycle:

```text
Learn → Practice → Investigate → Document
```

---

# 📊 Measuring Progress

Do not measure yourself only by:

- videos watched;
- certificates collected;
- tools installed;
- CTF flags completed.

Measure whether you can:

| Question | Target |
|---|---|
| Explain it? | Yes |
| Build it? | Yes |
| Reproduce it safely? | Yes |
| Troubleshoot it? | Yes |
| Explain the impact? | Yes |
| Explain detection? | Yes |
| Recommend remediation? | Yes |
| Document it professionally? | Yes |

### A useful rule

> **If you can reproduce it, troubleshoot it, explain it and defend against it, you probably understand it.**

---

# ❌ Common Mistakes

| Mistake | Better Approach |
|---|---|
| Starting with "hacking tools" | Start with networking and systems |
| Skipping networking | Make TCP/IP a priority |
| Copying commands | Understand every command you use |
| Collecting certificates | Build practical ability first |
| Only doing CTFs | Add labs, reports and administration |
| Ignoring Windows | Learn enterprise identity |
| Ignoring web security | Learn HTTP and application architecture |
| Ignoring defense | Study telemetry and detection |
| Never writing reports | Document every meaningful project |
| Publishing sensitive material | Publish sanitized work only |

---

# 🎤 Interview Preparation

## Networking

Be ready to explain:

- TCP vs UDP;
- DNS;
- HTTP/HTTPS;
- subnetting;
- NAT;
- routing;
- firewalls;
- TLS.

## Linux

Know:

- permissions;
- processes;
- services;
- users/groups;
- networking;
- logs.

## Windows

Know:

- services;
- PowerShell;
- processes;
- permissions;
- Event Logs.

## Active Directory

Know:

- domain controllers;
- Kerberos;
- LDAP;
- groups;
- GPO;
- ACLs;
- trusts.

## Web

Know:

- sessions;
- cookies;
- authentication;
- authorization;
- APIs;
- OWASP risks.

## Security

Know the difference between:

- threat vs vulnerability;
- vulnerability vs risk;
- authentication vs authorization;
- hashing vs encryption;
- detection vs prevention.

---

# 🧠 The Questions That Build Real Skill

For every topic, ask:

1. **What is it?**
2. **Why does it exist?**
3. **How does it work?**
4. **What assumptions does it make?**
5. **What can go wrong?**
6. **How would I identify the problem?**
7. **How could I validate it safely?**
8. **What evidence would I collect?**
9. **How could a defender detect it?**
10. **How should it be fixed?**

If you can answer these without blindly following a tutorial, you are moving from memorization toward understanding.

---

# ✅ Red Team Readiness Checklist

### Foundations

- [ ] Computer fundamentals
- [ ] TCP/IP
- [ ] DNS
- [ ] HTTP
- [ ] Linux
- [ ] Windows
- [ ] Virtualization

### Security

- [ ] CIA triad
- [ ] Authentication
- [ ] Authorization
- [ ] Cryptography basics
- [ ] Vulnerability concepts
- [ ] Security controls
- [ ] Logging

### Programming

- [ ] Python
- [ ] Bash
- [ ] PowerShell
- [ ] SQL
- [ ] JavaScript basics

### Offensive

- [ ] Reconnaissance
- [ ] Enumeration
- [ ] Web security
- [ ] Vulnerability validation
- [ ] Linux privilege concepts
- [ ] Windows privilege concepts
- [ ] Active Directory
- [ ] Cloud IAM

### Professional

- [ ] Scope awareness
- [ ] Evidence collection
- [ ] Report writing
- [ ] Risk communication
- [ ] Detection awareness
- [ ] Remediation recommendations
- [ ] Legal authorization

---

# 📚 Core Resources

Use this as the roadmap's permanent bookmark list. The phase-specific sections above tell you **when** to use these resources.

### Official references

- [OWASP](https://owasp.org/) — application security
- [OWASP Web Security Testing Guide](https://owasp.org/www-project-web-security-testing-guide/) — web testing methodology
- [PortSwigger Web Security Academy](https://portswigger.net/web-security) — free web-security labs
- [MITRE ATT&CK](https://attack.mitre.org/) — adversary techniques
- [MITRE ATLAS](https://atlas.mitre.org/) — AI security threats
- [NIST CSF](https://www.nist.gov/cyberframework) — cybersecurity framework
- [NIST SP 800-115](https://csrc.nist.gov/pubs/sp/800/115/final) — technical security testing
- [CIS Controls](https://www.cisecurity.org/controls) — practical security controls
- [Microsoft Learn](https://learn.microsoft.com/) — Windows, AD, Azure and identity
- [AWS Security](https://docs.aws.amazon.com/security/) — AWS security reference

### High-value GitHub repositories

| Repository | Use it for |
|---|---|
| [PayloadsAllTheThings](https://github.com/swisskyrepo/PayloadsAllTheThings) | Web/pentesting reference |
| [HackTricks](https://github.com/HackTricks-wiki/HackTricks) | Broad offensive-security reference |
| [GOAD](https://github.com/Orange-Cyberdefense/GOAD) | Active Directory lab |
| [InternalAllTheThings](https://github.com/swisskyrepo/InternalAllTheThings) | Internal/AD reference |
| [BloodHound](https://github.com/SpecterOps/BloodHound) | Identity/AD graph analysis |
| [Juice Shop](https://github.com/juice-shop/juice-shop) | Vulnerable web application lab |
| [vAPI](https://github.com/roottusk/vapi) | API security lab |
| [AWSGoat](https://github.com/ine-labs/AWSGoat) | Cloud security lab |
| [Atomic Red Team](https://github.com/redcanaryco/atomic-red-team) | Detection/security validation |
| [MITRE CALDERA](https://github.com/mitre/caldera) | Adversary emulation |
| [Ghidra](https://github.com/NationalSecurityAgency/ghidra) | Reverse engineering |
| [Volatility 3](https://github.com/volatilityfoundation/volatility3) | Memory analysis |

### Books worth keeping nearby

- *The Linux Command Line* — William Shotts
- *Computer Networking: A Top-Down Approach* — Kurose & Ross
- *Black Hat Python* — Justin Seitz & Tim Arnold
- *The Web Application Hacker's Handbook* — Dafydd Stuttard & Marcus Pinto
- *Real-World Bug Hunting* — Peter Yaworski
- *Practical Malware Analysis* — Michael Sikorski & Andrew Honig
- *Windows Internals* — Pavel Yosifovich et al.
- *The Practice of Network Security Monitoring* — Richard Bejtlich

### Hands-on platforms

- [TryHackMe](https://tryhackme.com/) — guided learning
- [Hack The Box](https://www.hackthebox.com/) — machines and advanced labs
- [PortSwigger Academy](https://portswigger.net/web-security) — web security
- [OverTheWire](https://overthewire.org/wargames/) — Linux/security challenges
- [picoCTF](https://picoctf.org/) — CTF practice
- [pwn.college](https://pwn.college/) — systems/exploitation learning
- [CTFtime](https://ctftime.org/) — CTF calendar and competitions
- [OffSec Proving Grounds](https://www.offsec.com/labs/proving-grounds/) — pentesting labs

> **Resource quality rule:** prefer official documentation and maintained projects. A GitHub repository is useful because it is popular, but popularity alone does not make a technique correct or safe. Check maintenance, scope and licensing before relying on a resource.

# ❓ FAQ

### Do I need programming before starting?

No. Start with networking and operating systems, then build programming gradually. Python is the best general-purpose starting point for many security learners.

### Do I need Linux?

Yes. You should become comfortable with the Linux command line and basic administration.

### Do I need Windows?

Yes. Especially if your long-term goal includes enterprise penetration testing or red teaming.

### Do I need networking?

Absolutely. Strong networking knowledge makes later security topics substantially easier.

### Should I start with Security+?

It can be a good structured security foundation for beginners. Pair it with practical labs rather than studying only for the exam.

### Should I immediately start OSCP?

Usually not. Build networking, Linux, Windows, web and practical lab experience first.

### Is CEH enough for red teaming?

No single certification makes someone a red-team operator. Practical skill, experience, judgment and tradecraft matter.

### Is red teaming just penetration testing?

No. Red teaming generally involves broader objectives, adversary simulation, detection awareness and organizational response.

### Can I learn this for free?

Yes. A substantial amount of high-quality material and hands-on practice is available without paying for every course.

### Do I need an expensive computer?

No. A modest machine can support a useful beginner lab. More RAM and storage become helpful as the lab grows.

---

# 🧭 From Learner to Operator

Think about progression in stages:

| Stage | Description |
|---|---|
| **Consumer** | Watches security content |
| **Student** | Understands concepts |
| **Practitioner** | Reproduces concepts in labs |
| **Problem Solver** | Troubleshoots unfamiliar situations |
| **Professional** | Performs structured assessments and reports |
| **Operator** | Reasons about objectives, attack paths, constraints and detection |

The purpose of this roadmap is to move through those stages deliberately.

---

# 🔥 The Principle I Would Keep Throughout the Roadmap

> **Don't memorize the attack. Understand the condition that makes the attack possible.**

If you understand the condition, you can:

- recognize it;
- investigate it;
- validate it;
- explain it;
- detect it;
- remediate it;
- recognize related weaknesses.

That is much more durable than memorizing another tool command.

---

# 🚀 Recommended Order

```text
01  Computer Fundamentals
02  Networking
03  Linux
04  Windows
05  Security Fundamentals
06  Python
07  Bash + PowerShell
08  HTTP + Web Architecture
09  OWASP
10  Reconnaissance
11  Enumeration
12  Vulnerability Analysis
13  Privilege Escalation Concepts
14  Active Directory
15  Internal Networks
16  Cloud
17  Identity & IAM
18  Adversary Simulation
19  OPSEC + Detection
20  Reporting
21  Specialization
22  Certification
23  Portfolio
24  Internship / Job
25  Continuous Learning
```

---

# 🏁 Final Note

Cybersecurity is not a race.

You will encounter people who know more than you, have more certifications, or have been practicing for years longer. That is normal.

Focus on building the underlying mental model.

Learn the protocol.

Build the environment.

Break it safely.

Read the logs.

Figure out why it broke.

Fix it.

Write down what happened.

Then do it again.

> **Learn the technology first. Understand the attack surface second. Validate safely. Think like the defender. Document everything.**

That is the foundation of real offensive-security capability.

---

## 👤 Author

**Fawad Qureshi**  
**Focus:** Red Team / Offensive Security  
**Edition:** 2026

### Purpose

This roadmap is intended for:

- cybersecurity education;
- authorized security testing;
- personal labs;
- CTFs;
- research;
- professional development.

> ⚠️ **Authorized-use only:** Never test systems you do not own or have explicit permission to assess.
