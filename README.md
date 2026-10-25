# 🦉 ODNSHunt

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OReconnaissance-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.1-cyan?style=flat-square"/>
</p>

> **ODNSHunt** — Fast DNS Subdomain Enumerator ║

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

ODNSHunt is a fast multi-threaded DNS subdomain enumerator for authorised reconnaissance and attack-surface mapping. It supports wordlist brute force, optional CT-log harvest, recursive modes, and JSON export so teams can inventory DNS names belonging to domains they own or are contracted to test.

---

## ✨ Features

- Wordlist-driven subdomain brute force with configurable threads and timeout
- Custom DNS resolver selection and request delay controls
- Optional Certificate Transparency harvest via --ct
- Deep and recursive scan modes for broader discovery
- JSON output path for downstream tooling
- Interactive menu or fully non-interactive CLI via --target / --no-menu

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./ODNSHunt -t example.com -w wordlist.txt --threads 50
./ODNSHunt -t example.com --ct --output results.json
./ODNSHunt -t example.com --deep --server 1.1.1.1 --no-menu
./ODNSHunt --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
