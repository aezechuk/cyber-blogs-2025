## Overview
CISA has added two critical vulnerabilities affecting Commvault's software to its Known Exploited Vulnerabilities (KEV) catalog. The first flaw, CVE-2025-3928, impacts the Commvault Web Server and allows remote, authenticated attackers to create and execute webshells on compromised systems. This high-severity vulnerability has a CVSS score of 8.7 enables attackers to maintain persistent access and execute arbitrary commands with the privileges of the web server. The second flaw, CVE-2025-34028, affects the Commvault Command Center installation and allows remote attackers to execute arbitrary code without authentication. This critical security flaw has a CVSS score of 10.0 and arises from a path traversal issue in the deployWebpackage.do endpoint, enabling attackers to upload malicious ZIP files that result in remote code execution.

Exploitation of these vulnerabilities has been observed in real-world attacks. Threat actors leverage authenticated user credentials to deploy webshells via the Commvault Web Server flaw, leading to complete server compromise, data exposure, and service disruption. The Command Center vulnerability has been exploited through server-side request forgery (SSRF), allowing attackers to upload and execute malicious files without authentication.
- The web server flaw is fixed in versions 11.36.46, 11.32.89, 11.28.141, and 11.20.217 for Windows and Linux platforms
- The command center vulnerability affects Command Center Innovation Release: 11.38.0-11.38.19 and is fixed in versions 11.38.20 and 11.38.25

### Why it matters:
Commvault's data protection and backup solutions are utilized by more than 100,000 organizations globally. These clients represent a diverse array of sectors, such as IT services, healthcare, education, and financial services. They depend on Commvault's robust data management features to protect their vital information and maintain seamless operations. Commvault has released patches for the Web Server flaw (CVE-2025-3928) and rotated affected credentials, collaborating with cybersecurity firms, the FBI, and CISA to address the issue. For the Command Center vulnerability (CVE-2025-34028), Commvault advises customers to upgrade to the latest versions or isolate affected systems if immediate patching is not possible.

### References
- [CSO Online: Critical Commvault SSRF Could Allow Remote Code Execution](https://www.csoonline.com/article/3970946/critical-commvault-ssrf-could-allow-attackers-to-execute-code-remotely.html)
- [CybersecurityNews: CISA Warns of Commvault Web Server Flaw](https://cybersecuritynews.com/cisa-commvault-web-server-flaw/)
- [watchTowr Labs: Fire in the Hole — Breaking the Vault: Commvault RCE (CVE-2025-34028)](https://labs.watchtowr.com/fire-in-the-hole-were-breaching-the-vault-commvault-remote-code-execution-cve-2025-34028/)

