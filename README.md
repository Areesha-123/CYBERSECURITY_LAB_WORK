
# Kali Linux Cybersecurity Assessment Laboratory

## 🛡️ Project Overview
This repository documents a series of hands-on laboratory tasks focused on web application security assessment and ethical hacking. Using **Kali Linux**, I conducted a structured evaluation of a target environment to identify vulnerabilities, map infrastructure, and recommend remediation strategies.

## 🧪 Laboratory Tasks & Methodologies
The assessment was divided into several critical phases of the penetration testing lifecycle:

### 1. Reconnaissance & OSINT (Passive)
Gathering information about the target without direct interaction to map its public footprint.
* [cite_start]**WHOIS:** Domain registration mapping and identifying name servers[cite: 14].
* [cite_start]**nslookup:** Querying DNS servers to retrieve IP addresses and records[cite: 14].
* [cite_start]**DNSenum:** Enumerating subdomains and DNS records for infrastructure mapping[cite: 18].

### 2. Active Scanning & Target Enumeration
Interrogating the target system to discover active services and potential entry points.
* [cite_start]**Nmap:** Service discovery and port scanning (identified 4 open ports)[cite: 18, 29].
* [cite_start]**SSLScan:** Analyzing SSL/TLS configurations to find weak ciphers and outdated protocols[cite: 18].
* [cite_start]**WhatWeb & Wafw00f:** Tech stack fingerprinting and Web Application Firewall (WAF) detection[cite: 22, 23].

### 3. Web Application Analysis
Probing the application layer for hidden content and common web vulnerabilities.
* [cite_start]**Gobuster:** Directory brute-forcing to uncover hidden files like `/admin` and `/uploads`[cite: 26, 29].
* [cite_start]**Skipfish:** Automated vulnerability scanning for XSS and Information Disclosure[cite: 26, 29].
* [cite_start]**WPScan:** CMS-specific auditing for WordPress vulnerabilities[cite: 26].

### 4. Exploitation & Forensic Research
* [cite_start]**Metasploit Framework:** Reviewing and verifying potential exploits (e.g., PHP-based RCE) in a controlled environment[cite: 29].
* **Social Engineering Toolkit (SET):** (Add specific details here if you performed phishing or credential harvesting simulations).
* **Digital Forensics:** (Add specific tools used, such as Autopsy or Sleuth Kit, if applicable to your tasks).

## 📊 Summary of Findings
| Phase | Tool | Risk Level | Key Finding |
| :--- | :--- | :--- | :--- |
| Recon | WHOIS/nslookup | Low | [cite_start]Domain mapping and DNS records [cite: 29] |
| Scanning | Nmap | Medium | [cite_start]4 Open Ports detected [cite: 29] |
| Crypto | SSLScan | Medium | [cite_start]Weak SSL/TLS protocols enabled [cite: 29] |
| Web | Gobuster | Medium | [cite_start]Unlisted directories (/admin, /uploads) found [cite: 29] |
| Analysis| Skipfish | Med-High | [cite_start]Potential XSS and Info Disclosure [cite: 29] |
| Exploit | Metasploit | Medium | [cite_start]Verified RCE vulnerability via PHP exploit [cite: 29] |

## 🚀 Key Recommendations
* [cite_start]**Harden Encryption:** Disable weak SSL/TLS ciphers and enforce modern standards[cite: 31].
* [cite_start]**Reduce Attack Surface:** Close unnecessary open ports and services[cite: 31].
* [cite_start]**Access Control:** Secure sensitive hidden directories with strong authentication[cite: 31].
* [cite_start]**Continuous Monitoring:** Perform regular patching and periodic security audits[cite: 31].

## ⚖️ Ethical Disclaimer
These tasks were performed strictly for educational purposes on authorized targets. [cite_start]All activities followed ethical hacking principles, and no unauthorized access or damage occurred[cite: 11, 12].

## 👥 Prepared By
* [cite_start]**Areesha Raheel** [cite: 1]
