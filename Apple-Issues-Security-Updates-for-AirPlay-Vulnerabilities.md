## Overview
Apple has rolled out security updates to address 23 vulnerabilities disclosed by security researchers. These flaws, affecting the Apple AirPlay protocol, can be exploited individually or in combination for greater impact. Notable vulnerabilities include CVE-2025-24252, a use-after-free flaw that allows attackers to corrupt process memory, and CVE-2025-24206, an authentication bypass enabling unauthorized access. When exploited together, these vulnerabilities can achieve zero-click remote code execution (RCE), allowing attackers to take control of devices without user interaction.

Oligo Security researchers have dubbed this set of vulnerabilities "AirBorne," highlighting their impact on wireless networks and peer-to-peer connections. While RCE is the most prominent attack vector, this collection of vulnerabilities can facilitate a range of attacks on various Apple devices, including third-party devices using the AirPlay software development kit (SDK).

### Why it matters: 
During Apple's January 2025 earnings call, CEO Tim Cook announced a record high of 2.35 billion active Apple devices globally. These vulnerabilities affect both enterprise and individual users. Customers choose Apple not only for its aesthetic appeal but also for its perceived security benefits. Apple advises users to enable automatic software updates and restrict AirPlay settings to reduce the attack surface. It is crucial to update all devices that could be running the AirPlay SDK, including smart TVs, audio systems, and CarPlay-enabled vehicles.

### References
- [BleepingComputer: Apple “AirBorne” Flaws Can Lead to Zero-Click AirPlay RCE Attacks](https://www.bleepingcomputer.com/news/security/apple-airborne-flaws-can-lead-to-zero-click-airplay-rce-attacks/)
- [SecurityWeek: AirPlay Vulnerabilities Expose Apple Devices to Zero-Click Takeover](https://www.securityweek.com/airplay-vulnerabilities-expose-apple-devices-to-zero-click-takeover/)
- [Oligo Security: AirBorne — Zero-Click AirPlay Vulnerabilities Explained](https://www.oligo.security/blog/airborne)
