# 🌐 ODNSHunt

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux%20%2F%20Windows-informational?style=flat-square&logo=linux&logoColor=white&color=0a0c10"/>
  <img src="https://img.shields.io/badge/Category-ORec%20%2F%20DNS-cyan?style=flat-square"/>
  <img src="https://img.shields.io/badge/Dependencies-None%20(stdlib)-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-v2.0-cyan?style=flat-square"/>
</p>

> **ODNSHunt** is an advanced multi-threaded DNS enumeration tool for subdomain discovery via brute-force wordlist. It supports A/AAAA records, wildcard detection, recursive scanning, live results, and exports to JSON, CSV, and TXT.

**No external dependencies — pure stdlib.**

---

## 📌 Overview

ODNSHunt performs fast and reliable subdomain enumeration by resolving subdomains against a built-in wordlist (or custom wordlist). It detects wildcard DNS to reduce false positives and supports deep scanning with multiple record types.

Ideal for reconnaissance, attack surface mapping, and authorized security testing.

---

## 🖥️ Modules

| # | Module                | Description |
|---|-----------------------|-------------|
| **[1]** | **Quick Scan**        | Default wordlist + A records only |
| **[2]** | **Deep Scan**         | A + AAAA records, wildcard check, recursive mode |
| **[3]** | **Custom Scan**       | Load your own wordlist file + full configuration |
| **[4]** | **Record Lookup**     | Manual DNS lookup for a single hostname (A, AAAA, PTR, FQDN) |
| **[5]** | **Wordlist Mgr**      | Preview and manage wordlist files |
| **[6]** | **Export Results**    | Save last scan to JSON / CSV / TXT |

---

## 📊 Key Features

- **Multi-threaded Brute-force** — Configurable threads for speed
- **Wildcard Detection** — Automatically detects and flags wildcard DNS
- **Multiple Record Types** — A (IPv4), AAAA (IPv6), with deep mode
- **Recursive Scanning** — Optional sub-subdomain discovery
- **Rate Limiting** — Delay and random jitter for stealth
- **Live Colored Results** — Real-time output with [WC] wildcard tags
- **Export Formats** — JSON (structured), CSV (spreadsheet), TXT (human-readable)
- **Built-in Wordlist** — 150+ common subdomain prefixes (admin, api, dev, mail, etc.)
- **Pure Python stdlib** — No extra packages required

---

## ⚙️ Requirements

- **No dependencies** — Uses only Python standard library (`socket`, `threading`, `queue`, etc.)

**Standalone executable** — Runs as `./ODNSHunt` when built with PyInstaller.

---

## 🚀 Usage

```bash
./ODNSHunt

📁 Output

Live Terminal — Real-time colored results showing subdomain, IPs, and wildcard status
Summary — Total found, real hits, wildcard matches, unique IPs, elapsed time
Export Files:
onextdns_<domain>_<timestamp>.json — Full structured data
onextdns_<domain>_<timestamp>.csv — Spreadsheet format
onextdns_<domain>_<timestamp>.txt — Human-readable report



📦 Part of OwlSec Toolkit
This tool is part of the OwlSec suite — a collection of 300+ security and privacy tools.
🔗 owlsec.org

©️ License
Proprietary — © Khaled S. Haddad
Tools are distributed as pre-built executables. Source code is proprietary.
AUTHORISED RECONNAISSANCE & SECURITY TESTING USE ONLY
