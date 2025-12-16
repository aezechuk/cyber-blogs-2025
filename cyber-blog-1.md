## Overview
The Morphing Meerkat phishing kit is a sophisticated phishing-as-a-service platform that targets over 100 brands by exploiting DNS mail exchange records. This kit uses DNS-over-HTTPS to bypass traditional DNS filters and monitoring tools, making it harder for security software to detect the threat. The attack typically begins with a convincing email that appears to come from widely recognized brands, urging the recipient to take immediate action. When the user clicks on the link, they are redirected through a series of compromised sites, eventually landing on a fake login page tailored to their email provider.

The phishing kit dynamically generates these counterfeit login pages based on the victim's email domain, making them nearly indistinguishable from the real ones. If the user enters their credentials, the information is transmitted to the attackers, often in real-time via tools like Telegram bots. 

Active since at least 2020, according to InfoBlox, Morphing Meerkat has evolved to be more scalable, stealthy, and easy to use. The phishing kit incorporates anti-analysis measures, such as prohibiting the use of mouse right-click and keyboard hotkey combinations, to prevent users from saving or viewing the web page source code. The kit also translates phishing content into multiple languages, targeting users worldwide. By leveraging DNS MX records, the phishing kit can accurately mimic login pages for various email providers, enhancing its effectiveness in tricking victims into submitting their credentials. 

### Additional key details:

- If a phishing kit does not recognize the MX record, it typically defaults to a Roundcube (open-source email software)
- About 50% of the traced emails originate from servers belonging to internet services provided by iomart (UK) and HostPapa (US)
- Four distinct collection methods have been identified: 
    - Email, 
    - PHP scripts on the same site, 
    - Remote data transfer via AJAX requests, 
    - Communication with text channels using web API hooks

### Why it matters: 
The evolution of phishing techniques underscores the need for organizations to stay vigilant and continuously update their security protocols to counter these advanced threats. Additionally, diligent monitoring of systems for suspicious activities and educating employees about phishing tactics can significantly reduce the likelihood of successful attacks.

### References 
- [BleepingComputer: Phishing-as-a-Service Uses DNS-over-HTTPS](https://www.bleepingcomputer.com/news/security/phishing-as-a-service-operation-uses-dns-over-https-for-evasion/)
- [The Hacker News: Morphing Meerkat Targets 100+ Brands](https://thehackernews.com/2025/03/new-morphing-meerkat-phishing-kit.html)
- [SecurityWeek: Morphing Meerkat Analysis](https://www.securityweek.com/morphing-meerkat-phishing-kits-target-over-100-brands/)
- [Infoblox: A Phishing Tale of DoH and DNS MX Abuse](https://blogs.infoblox.com/threat-intelligence/a-phishing-tale-of-doh-and-dns-mx-abuse/)
