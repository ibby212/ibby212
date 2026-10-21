# Ibaad Shams

### Blue team · SOC & detection engineering · Computer Science student at EPITA Paris

BSc Computer Science student at **EPITA** (2024–2027), working on the defensive side of security: monitoring, detection rules and incident triage. Most of what's here is labs I built, attacked, and then wrote the detection rules for.

**Looking for a 6-month SOC / detection engineering internship (stage de fin d'études) starting February or March 2027, in Paris.**

---

## Projects

### [Network Attack & Detection Lab: OPNsense + Suricata IDS](https://github.com/ibby212/suricata-opnsense-detection-lab)
A two-person attack/detection lab inside a four-student group, where I ran the **defender** side. I hosted OPNsense, a vulnerable DVWA target and the **Suricata** sensor while a teammate launched live web attacks across a Tailscale link. I wrote **five custom Suricata rules** (SIDs 9000010–9000040) for command injection, web shell, local file inclusion, DNS tunnelling and raw-TCP shell output, mapped to **MITRE ATT&CK** so they match the result of an attack rather than one payload, then measured their false positives against normal browsing and tuned them to zero while the real attack still fired. For the capstone I rebuilt the incident timeline from Suricata's `eve.json`: command injection → web shell → bind shell → DNS exfiltration, each stage with its SID and timestamp. Two things worth noting: a reverse shell blocked on port 4444 still left over HTTPS on 443, and DNS tunnelling was caught even though the queries never leave the resolver.

`Suricata` `OPNsense` `DVWA` `Network IDS` `MITRE ATT&CK` `Detection engineering`

### [IAM Labs: Keycloak, midPoint, LDAP, Entra ID](https://github.com/ibby212/iam-keycloak-midpoint-labs)
Seven identity and access management labs: MFA and brute-force lockout, HR-driven joiner/mover/leaver provisioning, Segregation of Duties, access certification, OIDC SSO and federation with Google and Microsoft Entra ID. Each lab ends with an **attacker view / defender view** mapped to MITRE ATT&CK and the signals a SOC should alert on.

`Keycloak` `midPoint` `OpenLDAP` `OIDC` `Entra ID` `MITRE ATT&CK` `Docker`

### [OSPF, BGP & NAT Network Lab](https://github.com/ibby212/ospf-bgp-nat-network-lab)
A two-autonomous-system network built by hand in Cisco Packet Tracer: VLSM addressing, multi-area OSPF, eBGP peering, PPP with CHAP, ACLs, static NAT and PAT, plus DNS and mail servers. I then reviewed it as if I were responsible for it, and documented **5 security and design findings** with the fix for each: private IP leaked in public DNS, NAT exposing every port, no management-plane hardening.

`Cisco IOS` `OSPF` `BGP` `NAT` `ACLs` `Packet Tracer` `Network security`

---

## Tools & skills

![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat&logo=gnubash&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Splunk](https://img.shields.io/badge/Splunk-000000?style=flat&logo=splunk&logoColor=white)
![Suricata](https://img.shields.io/badge/Suricata-EF6C00?style=flat)
![Keycloak](https://img.shields.io/badge/Keycloak-4D4D4D?style=flat&logo=keycloak&logoColor=white)
![Cisco](https://img.shields.io/badge/Cisco_IOS-1BA0D7?style=flat&logo=cisco&logoColor=white)

**Security domains:** `SOC / alert triage` `SIEM` `Network IDS` `Detection rules` `Identity & Access Management` `Routing & network security` `MITRE ATT&CK`

---

## Certifications

- TryHackMe **SOC Level 1**
- Fortinet **NSE 1**
- CNIL **L'atelier RGPD**

---

## Contact

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ibaad-shams/)

🇬🇧 English (C1) · 🇫🇷 French (B1) · 🇮🇳 Hindi (Native) · Urdu (Native)
