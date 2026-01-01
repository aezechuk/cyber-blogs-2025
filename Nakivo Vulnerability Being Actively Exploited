## Overview
The Cybersecurity and Infrastructure Security Agency (CISA) has reported that a critical vulnerability in Nakivo Backup and Replication software, identified as CVE-2024-48248, is being actively exploited. Although Nakivo patched this vulnerability in early November 2024, it remains a significant threat to systems that have not been updated. This security flaw has a CVSS 3.1 score of 8.6 out of 10. 

### Key details include:
- The vulnerability allows for absolute path traversal via the getImageByPath function to the /c/router endpoint, potentially leading to remote code execution across the enterprise.
- It affects all versions of Nakivo Backup & Replication up to 10.11.3.86570.
- Nakivo has released a patch in version 11.0.0.88174 to address this issue, and users are strongly urged to upgrade immediately.

WatchTowr Labs, which originally disclosed the bug to Nakivo in October 2024, published a proof-of-concept exploit and a vulnerability research paper in late February 2025, detailing how the vulnerability was discovered. This flaw allows attackers to read arbitrary files on the affected system without authentication, potentially exposing sensitive data such as configuration files, backups, and credentials, leading to data breaches or further security compromises. CISA has issued an advisory about the vulnerability being exploited in the wild and has mandated that Federal Civilian Executive Branch (FCEB) agencies implement the necessary security patches by April 9, 2025.


### Why it matters:
Nakivo Backup & Replication is a vital tool for many organizations, providing essential data protection and recovery capabilities. Due to its extensive integration capabilities within an organization's ecosystem, including cloud services, this vulnerability could allow an attacker to gain access to the entire infrastructure. It is strongly recommended to upgrade Nakivo Backup and Replication to version 11.0.0.88174 or later.
Regularly review system logs for unusual or unauthorized access attempts, focusing on unexpected file access activities. Enhance network security by implementing network segmentation to limit backup systems' exposure to untrusted networks. Apply firewall rules to restrict access to trusted users and use strong authentication mechanisms to secure backup systems.

### References
- [The Hacker News: CISA Adds Exploited NAKIVO Backup & Replication Vulnerability to KEV Catalog](https://thehackernews.com/2025/03/cisa-adds-nakivo-vulnerability-to-kev.html)
- [SecurityWeek: CISA Warns of Actively Exploited NAKIVO Vulnerability](https://www.securityweek.com/cisa-warns-of-exploited-nakivo-vulnerability/)
- [watchTowr Labs: Deep Dive Into NAKIVO Backup & Replication Vulnerability (CVE-2024-48248)](https://labs.watchtowr.com/the-best-security-is-when-we-all-agree-to-keep-everything-secret-except-the-secrets-nakivo-backup-replication-cve-2024-48248/)
