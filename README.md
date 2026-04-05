# 🦅 OHawkEye

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux%20%2F%20Windows-informational?style=flat-square&logo=linux&logoColor=white&color=0a0c10"/>
  <img src="https://img.shields.io/badge/Category-ORec%20%2F%20Automated%20Recon-cyan?style=flat-square"/>
  <img src="https://img.shields.io/badge/Dependencies-nmap-yellow?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-v1.0-cyan?style=flat-square"/>
</p>

> **OHawkEye** is an automated multi-phase reconnaissance framework. It performs port scanning (TCP/UDP), service enumeration, vulnerability checking, and generates rich reports in JSON, HTML, Markdown, and TXT formats.

**Plugins for Web, SMB, FTP, SSH, SMTP, DNS + vuln scanning with nmap --script vuln and nikto.**

---

## 📌 Overview

OHawkEye runs a complete reconnaissance workflow:
- **Phase 1**: Port scanning (TCP + optional UDP)
- **Phase 2**: Service enumeration (Web, SMB, FTP, SSH, SMTP, DNS)
- **Phase 3**: Vulnerability scanning (nmap-vuln + nikto)
- **Reports**: JSON, HTML, Markdown, TXT with findings and recommendations

Ideal for automated network reconnaissance and purple team exercises.

---

## 🖥️ Modules

| # | Module                  | Description |
|---|-------------------------|-------------|
| **[1]** | **New Scan**            | Launch full recon against target(s) |
| **[2]** | **View Results**        | Display findings from last scan |
| **[3]** | **Reports**             | Generate/re-export reports |
| **[4]** | **Settings**            | Ports, threads, timeouts, phases |
| **[5]** | **Tool Check**          | Verify availability of external tools |

---

## 📊 Key Features

- **Multi-Phase Automated Recon** — Port scan → Enumeration → Vulnerability check
- **Service-Specific Plugins**:
  - Web (whatweb + gobuster/dirb)
  - SMB (enum4linux + smbclient)
  - FTP (anonymous login check)
  - SSH (banner + ssh-audit)
  - SMTP (smtp-user-enum + relay test)
  - DNS (zone transfer + open resolver check)
- **Vuln Scanning** — nmap --script vuln + nikto
- **Risk-Based Findings** — CRITICAL / HIGH / MEDIUM / LOW with recommendations
- **Rich Reporting** — JSON, HTML (with CSS), Markdown, TXT
- **Configurable** — Ports, UDP, threads, timeouts, OS detection

---

## ⚙️ Requirements

- **nmap** (required)
  ```bash
  sudo apt install nmap
  chmod +x OHawkEye
  sudo ./OHawkEye

  📦 Part of OwlSec Toolkit
This tool is part of the OwlSec suite — a collection of 300+ security and privacy tools.
🔗 owlsec.org

©️ License
Proprietary — © Khaled S. Haddad
Tools are distributed as pre-built executables. Source code is proprietary.
AUTHORISED SECURITY TESTING USE ONLY
