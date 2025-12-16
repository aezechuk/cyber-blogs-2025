## Overview
Cybercrime group known as FIN6, active since 2012 and known for targeting point-of-sales (POS) systems, has launched a new phishing campaign targeting recruiters on LinkedIn and other job platforms. The attackers impersonate job applicants and trick recruiters into downloading malware disguised as resumes. The actively used lure aimed at Human Resources (HR) professionals, leverages social engineering tactics and cloud-hosted websites trusted by enterprise network filters to evade detection.

The scheme begins when a recruiter receives a message from a fake applicant, often with a convincing LinkedIn profile. Instead of attaching a resume, the attacker shares a non-clickable link to a personal website hosted on Amazon Web Services or another trusted cloud provider. While completing a CAPTCHA, environmental and behavioral checks ensure that only intended victims can access their malicious landing pages, which are masked as professional portfolios. The recruiter is then prompted to download a ZIP file containing a malicious Windows shortcut (.lnk) file alongside an image file serving as a diversion. When opened, the file installs a JavaScript backdoor known as More_eggs, which can steal credentials, execute remote commands and enable additional attacks like ransomware. The attack affects Windows users as connections originating from non-Windows operating systems like Linux or macOS or VPNs are automatically redirected to harmless content, attempting to filter out researchers and automated scanners.

### Why it matters:
This campaign shows the growing threat of social engineering attacks and the vulnerability of corporate HR departments. With LinkedIn widely used for recruitment, the potential reach of the scam is significant. "FIN6's Skeleton Spider campaign shows how effective low-complexity phishing campaigns can be when paired with cloud infrastructure and advanced evasion," the researchers concluded. "By using realistic job lures, bypassing scanners, and hiding malware behind CAPTCHA walls, they stay ahead of many detection tools." Educate HR and recruitment teams on phishing tactics, avoid downloading resumes from unknown or unverified sources, and implement endpoint detection and response (EDR) tools. As attackers continue to exploit trust and routine workflows, cybersecurity awareness remains essential.

### References
- [CSO Online: FIN6 Exploits HR Workflows to Breach Corporate Defenses](https://www.csoonline.com/article/4005944/fin6-exploits-hr-workflows-to-breach-corporate-defenses.html)
- [BleepingComputer: FIN6 Hackers Pose as Job Seekers to Backdoor Recruiters’ Devices](https://www.bleepingcomputer.com/news/security/fin6-hackers-pose-as-job-seekers-to-backdoor-recruiters-devices/)
- [The Record: FIN6 Uses Recruitment Scam to Deploy More_eggs Backdoor](https://therecord.media/fin6-recruitment-scam-malware-campaign)
- [The Hacker News: FIN6 Uses AWS-Hosted Fake Resumes in New Malware Campaign](https://thehackernews.com/2025/06/fin6-uses-aws-hosted-fake-resumes-on.html)



