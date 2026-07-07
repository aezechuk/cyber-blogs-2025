## Overview
Security researcher Alvaro Balada disclosed a critical vulnerability in Grafana, an open-source data visualization platform, on May 15. The flaw, nicknamed “Grafana Ghost” and tracked as CVE-2025-4123, allows attackers to hijack user accounts by exploiting the platform’s plugin system. The attack targets users who click on malicious links, which triggers the installation of rogue plugins capable of executing arbitrary JavaScript. Public-facing Grafana instances with external plugin loading enabled are most at risk, but even Grafana servers not connected to the internet are at risk of blind attacks. While patches have been released, many systems remain unprotected.

The Grafana Ghost vulnerability is carried out through a chain of exploits initiated when attackers send a link that, when clicked, causes Grafana to load a plugin from an external server. The attack does not require prior access or authentication and can be used to bypass modern browser normalization mechanisms due to Grafana's JavaScript routing logic. Once installed, the plugin can change user credentials, access sensitive dashboards, and lock out legitimate users. Affected versions include Grafana 10.x through 12.0.1, especially those with plugin loading enabled and exposed to the internet.

### Why it matters: 
OX Security shared a Shodan query code to verify the number of Grafana instances still vulnerable, and a month later, nearly 47,000 instances remain unpatched. Thirty-six percent of the affected population missed the memo, running vulnerable versions that could still be exploited. Grafana is widely used in enterprise IT environments; a core tool for monitoring infrastructure. A successful exploit could expose critical operational data or disrupt services. Organizations are urged to patch their systems, audit plugin configurations, and restrict public access to reduce the risk of exploitation.

### References
- [CSO Online: Grafana “Ghost” XSS Flaw Exposes 47,000 Servers to Account Takeover](https://www.csoonline.com/article/4007522/grafana-ghost-xss-flaw-exposes-47000-servers-to-account-takeover.html)
- [BleepingComputer: Over 46,000 Grafana Instances Exposed to Account Takeover Bug](https://www.bleepingcomputer.com/news/security/over-46-000-grafana-instances-exposed-to-account-takeover-bug/)
- [Infosecurity Magazine: Over a Third of Grafana Instances Remain Vulnerable](https://www.infosecurity-magazine.com/news/over-third-grafana-instances/)

