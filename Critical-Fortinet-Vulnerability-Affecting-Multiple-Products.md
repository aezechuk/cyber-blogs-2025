## Overview
A critical security flaw identified in May 2025 has prompted Fortinet and CISA to issue urgent warnings to users of several of the company’s products. While there were multiple vulnerabilities recently made public, the most critical CVE-2025-32756 (CVSS 9.8), was discovered during internal reviews and confirmed by Fortinet’s Product Security Incident Response Team. It affects a range of systems including FortiVoice, FortiRecorder, FortiMail, FortiNDR, and FortiCamera. The Fortinet product team discovered the vulnerability based on threat actor activity that originated from the following IP address: 
- 198.105.127.124 
- 43.228.217.173 
- 43.228.217.82 
- 156.236.76.90 
- 218.187.69.244 
- 218.187.69.59

The flaw, a stack-based buffer overflow vulnerability, allows attackers to remotely execute code without needing to log in, making it especially dangerous for internet-facing devices. The exploit works by sending a specially crafted HTTP request that triggers a buffer overflow, allowing the attacker to take control of the system. Because the attack doesn’t require authentication, it can be launched by anyone with access to the network or exposed services. Organizations using outdated versions of the affected products are most at risk. Fortinet has observed this to be exploited in the wild on FortiVoice. Fortinet has provided detailed mitigation steps and continues to monitor for signs of exploitation.

### Why it matters:
Not only are Fortinet products widely used across industries, including government, healthcare, and enterprise networks, this vulnerability affects multiple products, making it a significant concern. An attacker could take full control of affected systems without needing credentials. Fortinet has released patches for this vulnerability and others such as, CVE-2025-22252 (CVSS score of 9.0), described as a missing authentication for critical function defect that could lead to TACACS+ authentication bypass. Customers are urged to update immediately.

### References
- [SecurityWeek: Fortinet Patches Zero-Day Exploited Against FortiVoice Appliances](http://securityweek.com/fortinet-patches-zero-day-exploited-against-fortivoice-appliances/)
- [The Hacker News: Fortinet Patches CVE-2025-32756 Zero-Day Actively Exploited in the Wild](https://thehackernews.com/2025/05/fortinet-patches-cve-2025-32756-zero.html)
- [BleepingComputer: Fortinet Fixes Critical Zero-Day Exploited in FortiVoice Attacks](https://www.bleepingcomputer.com/news/security/fortinet-fixes-critical-zero-day-exploited-in-fortivoice-attacks/)

