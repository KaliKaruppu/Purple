# Purple
Red+Blue
# 🔥 Purple Team Active Directory Lab – Red Team & Blue Team Operations

## 📌 Overview

Built and operated a complete Purple Team cybersecurity lab environment combining offensive security techniques with defensive monitoring and detection engineering.

This project focused on:

* Active Directory reconnaissance
* LDAP & Kerberos enumeration
* SMB security assessment
* SIEM visibility
* Sysmon telemetry analysis
* Splunk monitoring & troubleshooting
* Ethical adversary simulation inside an isolated lab

---

# 🏗️ Lab Architecture

```text
[Kali Linux Attacker]
        |
        |
[Windows Server / AD DC]
        |
[Windows 11 Endpoint]
        |
[Splunk Enterprise + Sysmon]
```

---

# 🛠️ Technologies Used

## Offensive Security

* Kali Linux
* Nmap
* CrackMapExec
* LDAP tools
* SMB enumeration
* Kerberos reconnaissance

## Defensive Security

* Splunk Enterprise
* Sysmon
* Windows Event Logs
* Active Directory monitoring

---

# 🎯 Objectives

* Simulate real-world AD reconnaissance
* Assess SMB hardening posture
* Perform LDAP enumeration
* Analyze Kerberos exposure
* Validate defensive controls
* Detect attacker activity using Splunk
* Practice Purple Team methodology

---

# 🔍 Reconnaissance & Enumeration Performed

## SMB Recon

Successfully identified:

* Domain Name
* Hostname
* SMB Signing Status
* SMBv1 Status
* OS Fingerprinting

### Findings

✅ SMB Signing Enabled
✅ SMBv1 Disabled
✅ Anonymous Share Enumeration Blocked

These controls significantly reduced common attack paths.

---

## LDAP Enumeration

Performed anonymous LDAP RootDSE enumeration.

Successfully identified:

* Domain Naming Contexts
* Forest & Domain Functional Levels
* LDAP Capabilities
* Kerberos Support
* Global Catalog Status

### Key Discovery

```text
DC=corp,DC=local
```

### Assessment

LDAP information disclosure was informational only and did not directly expose sensitive data.

---

## Kerberos Reconnaissance

Validated:

* Kerberos service exposure
* Port 88 availability
* AD authentication infrastructure

### Result

```text
88/tcp open kerberos-sec
```

Kerberos user enumeration attempts did not disclose usernames, indicating proper defensive handling.

---

# 🛡️ Blue Team & Detection Engineering

Integrated:

* Sysmon
* Splunk Enterprise
* Windows Event Logs

Performed:

* PowerShell telemetry analysis
* Process execution monitoring
* Authentication visibility testing
* Event correlation
* Recon activity tracking

---

# 📊 Purple Team Operations

Generated controlled administrative/recon activity:

* whoami
* ipconfig /all
* Get-Process
* LDAP queries
* SMB enumeration

Then validated visibility inside Splunk.

---

# 🔥 Key Skills Demonstrated

* Active Directory Security
* Purple Team Methodology
* SIEM Operations
* Threat Detection
* Windows Internals
* Network Enumeration
* LDAP & Kerberos Analysis
* Detection Engineering
* Sysmon Telemetry
* Splunk Troubleshooting

---

# 📚 Key Takeaways

This lab reinforced the importance of:

* Ethical security testing
* Detection-first mindset
* Understanding defensive controls
* Attack surface analysis
* Correlating offensive activity with telemetry

A major focus was learning how mature environments:

* harden SMB
* restrict enumeration
* expose minimal attack surface
* maintain monitoring visibility

---

# 🚀 Future Enhancements

Planned next steps:

* BloodHound integration
* ATT&CK mapping
* PowerShell detection analytics
* Scheduled task persistence detection
* Wazuh integration
* Sigma rule development
* Threat hunting dashboards

---

# ⚠️ Disclaimer

All activities were conducted in a personally owned isolated lab environment for educational and defensive security purposes only.



