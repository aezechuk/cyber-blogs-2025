Summary: 
Microsoft and the U.S. Cybersecurity and Infrastructure Security Agency (CISA) have confirmed active exploitation of two critical vulnerabilities in on-premises SharePoint Servers-CVE-2025-53770 and CVE- 2025-53771. The first, CVE-2025-53771, allows attackers to bypass authentication by spoofing a Referer header to mimic legitimate SharePoint workflows. Then, they exploit CVE-2025-53770, a remote code execution flaw rated 9.8 on the CVSS scale, to run malicious code. Together, the two vulnerabilities form the basis of the ToolShell exploit chain, which affects SharePoint Server 2016, 2019, and the Subscription Edition. 
The attack targets how SharePoint handles requests to layout pages, particularly /layouts/15/ToolPane.aspx?DisplayMode=Edit. By sending crafted HTTP POST requests to this endpoint, attackers exploit weaknesses in how configuration data is processed. This can expose the server's 
ASP.NET MachineKey settings, which are used to encrypt and validate authentication tokens and view 
state. With this information, attackers can forge tokens, impersonate users, and execute code remotely, 
without needing to log in. If the SharePoint server is accessible from the internet, the attack can be launched externally. 
Why it matters: 
These vulnerabilities are critical because they affect SharePoint, a platform used by the vast majority of 
Fortune 500 companies and numerous government agencies. The ToolShell campaign has already compromised more than 400 organizations, including U.S. federal entities and global enterprises. Security experts warn that any internet-facing SharePoint instance should be considered compromised 
unless proven otherwise. The ability to bypass authentication and extract cryptographic keys gives 
attackers long-term, privileged access to sensitive systems. Mitigation is essential: applying patches, rotating keys, and enhancing monitoring can prevent further exploitation and limit the damage from 
these sophisticated attack
