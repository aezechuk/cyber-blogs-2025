## Overview
Cybersecurity firm Wiz has uncovered an active cryptojacking campaign exploiting misconfigured DevOps tools, including Docker, HashiCorp Nomad, Consul and Gitea. The campaign, attributed to a threat actor known as JINX-0132, was disclosed in early June and marks the first known exploitation of Nomad misconfigurations in the wild. Attackers are using publicly accessible APIs to deploy XMRig, a cryptocurrency miner, across vulnerable, high-compute systems identified using Shodan and FOFA queries. A wide-range of tools have been targeted and many instances are still exposed due to misconfigurations.

The attackers scan the internet for exposed services and use legitimate open-source tools hosted on GitHub to avoid detection. Once access is gained, they deploy mining software that consumes significant computing resources. Docker instances with open APIs, Nomad clusters lacking access controls, unpatched Gitea servers, and Nomad job-queue API are among the most vulnerable. These attacks often use standard binaries instead of malware, leverage legit services and avoid attacker-controlled infrastructure. This "living-off-open-source" approach makes the campaign harder to detect and stop. 

### Why it matters:
The campaign is noteworthy because it targets core cloud infrastructure and tools like Docker that have permeated into majority of DevOps workflows. Compromised systems have been found running hundreds of clients, with stolen compute resources valued in the tens of thousands of dollars per month. These misconfiguration-based exploits, don’t require zero-day vulnerabilities. Security experts urge organizations to assess the security requirements for their environment and enable the appropriate mechanisms. Nomad's documentation for instance, explicitly states "Nomad is not secure by-default" and the proper configurations must be implemented, correctly. Avoid configurations for the purpose of convenience, apply patches, restrict API internet access and enforce strict access controls (ACLs). Minor lapses in configuration can lead to financial losses with big business impact.

### References
- [CSO Online: The High Cost of Misconfigured DevOps — Global Cryptojacking Hits Enterprises](https://www.csoonline.com/article/4000714/the-high-cost-of-misconfigured-devops-global-cryptojacking-hits-enterprises.html)
- [The Hacker News: New Cryptojacking Campaign Exploits Misconfigured DevOps Infrastructure](https://thehackernews.com/2025/05/new-self-spreading-malware-infects.html)
- [SecurityWeek: Cryptojackers Mine Monero via Exposed DevOps Tools](https://www.securityweek.com/cryptojackers-caught-mining-monero-via-exposed-devops-infrastructure/)
- [Wiz Research: JINX-0132 Cryptojacking Campaign Targeting Cloud and DevOps Environments](https://www.wiz.io/blog/jinx-0132-cryptojacking-campaign)


