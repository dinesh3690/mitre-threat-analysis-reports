# MITRE ATT&CK Threat Analysis Reports

A collection of structured threat intelligence reports analysing real-world cyberattacks using the MITRE ATT&CK framework. Each report maps attacker behaviour to specific tactics and techniques, identifies detection opportunities, and provides recommendations for SOC teams. This project demonstrates threat intelligence analysis skills at a graduate level — researching real attacks, thinking like an attacker, and communicating findings clearly for both technical and non-technical audiences.

---

## Reports

### Report 1 — WannaCry Ransomware (2017)
**Type:** Ransomware worm — nation-state attributed
**Threat Actor:** Lazarus Group (North Korea)
**Impact:** 200,000+ victims across 150 countries
**Key techniques:** EternalBlue exploitation, SMB lateral movement, shadow copy deletion, file encryption
**Folder:** `wannacry/`

### Report 2 — Medibank Healthcare Data Breach (2022)
**Type:** Data exfiltration — ransomware extortion
**Threat Actor:** REvil-linked Russian cybercriminal group
**Impact:** 9.7 million Australian healthcare records exposed
**Key techniques:** Stolen credentials, VPN access without MFA, network reconnaissance, data exfiltration
**Folder:** `medibank/`

---

## Methodology

Each report follows this structure:

1. **Attack Overview** — who, what, when, impact in plain English
2. **Attack Timeline** — step-by-step reconstruction of the attack chain
3. **MITRE ATT&CK Mapping** — each attacker action mapped to tactic and technique ID
4. **SOC Detection Opportunities** — what logs and alerts would have caught this
5. **Lessons Learned** — what the attack teaches defenders
6. **Recommendations** — specific controls to prevent or detect similar attacks

---

## Tools Used

| Tool | Purpose |
|------|---------|
| MITRE ATT&CK Navigator | Mapping attack techniques and generating visual attack chain maps |
| CISA Advisories | Primary source for WannaCry attack details |
| ACSC Advisories | Primary source for Medibank breach details |
| MITRE ATT&CK Framework | Technique identification and classification |

---

## Why These Two Attacks

**WannaCry** is the most recognised ransomware attack globally — appearing in almost every cybersecurity job interview and certification exam. Understanding it in depth demonstrates core threat intelligence competency.

**Medibank** is an Australian healthcare breach — directly relevant to the Adelaide cybersecurity job market where SA Health and healthcare organisations are major employers. The attack succeeded through credential theft and absence of MFA — two of the most common attack vectors in Australian SOC environments today. Following this breach, the Australian government mandated stricter Essential Eight compliance across healthcare organisations.

---

## MITRE ATT&CK Coverage

| Technique ID | Technique Name | WannaCry | Medibank |
|-------------|----------------|----------|---------|
| T1595.001 | Scanning IP Blocks | ✅ | |
| T1190 | Exploit Public-Facing Application | ✅ | |
| T1059.003 | Windows Command Shell | ✅ | |
| T1210 | Exploitation of Remote Services | ✅ | |
| T1027 | Obfuscated Files or Information | ✅ | |
| T1490 | Inhibit System Recovery | ✅ | |
| T1486 | Data Encrypted for Impact | ✅ | ✅ |
| T1078 | Valid Accounts | | ✅ |
| T1133 | External Remote Services | | ✅ |
| T1110 | Brute Force | | ✅ |
| T1021 | Remote Services | | ✅ |
| T1083 | File and Directory Discovery | | ✅ |
| T1041 | Exfiltration Over C2 Channel | | ✅ |

**Total techniques mapped: 13 across 2 reports**

---

## Skills Demonstrated

- Real-world attack research using authoritative sources (CISA, ACSC, MITRE)
- MITRE ATT&CK framework application — tactic and technique mapping
- Threat intelligence report writing for both technical and non-technical audiences
- SOC detection opportunity identification across multiple log sources
- Australian cybersecurity context awareness — Essential Eight, ACSC, Privacy Act implications
- Analytical thinking — root cause analysis and lessons learned documentation
