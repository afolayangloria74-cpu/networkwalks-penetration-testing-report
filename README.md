# networkwalks-penetration-testing-report
For cybersecurity
# Penetration Testing Report
### NETWORKWALKS - Batch B084D

**Intern:** Afolayan Gloria
**Intern ID:** NW-084-000
**Supervisor:** Waqas Karim, CCIE
**Date:** 13 November 2026

## Executive Summary

This report presents the results of a penetration test conducted on the domain **networkwalks.com**.

The test was carried out using only open-source and passive reconnaissance techniques. No active exploitation was performed.

The goal was to identify publicly exposed information, misconfigurations, and potential attack surfaces that an attacker could use.

## Scope

**Target Domain:** networkwalks.com
**Target IP:** 162.241.85.29
**Test Type:** Black-box, Passive Reconnaissance
**Tools Used:** WHOIS, Shodan, Google Hacking Database, DNS Enumeration, Ping, Traceroute, Zenmap

## Methodology

1.  **Information Gathering:** WHOIS lookup to identify domain owner and registrar.
2.  **Search Engine Recon:** Shodan and Google Hacking Database (GHDB) to find exposed data.
3.  **DNS Enumeration:** To map subdomains and mail servers.
4.  **Network Mapping:** Ping and Traceroute to check live host and network path.
5.  **Port Scanning:** Zenmap (Nmap) to identify open ports and services.

## Key Findings

| Finding | Risk |
| :--- | :--- |
| Domain uses Cloudflare protection | Low |
| 7 subdomains discovered | Info |
| Open Ports: 80, 443, 2083, 2087 | Medium |
| Server leaks version info | Low |
| SPF and DMARC records present | Good |

## Screenshots

All evidence screenshots are in the `screenshots` folder:

- WHOIS Lookup
- Shodan Search Result
- Google Hacking Database (GHDB)
- DNS Enumeration
- Ping Test
- Traceroute
- Zenmap Scan

## Recommendations

1.  Hide server version banners to reduce information leakage.
2.  Review open ports 2083 and 2087 - close if not needed.
3.  Enable DNSSEC for stronger DNS security.
4.  Continue regular vulnerability scanning.

## Conclusion

The domain **networkwalks.com** is well protected with Cloudflare and has no critical vulnerabilities found during passive testing. The medium-risk open ports should be reviewed to reduce attack surface.

---
**Report by Afolayan Gloria | NETWORKWALKS Intern**
