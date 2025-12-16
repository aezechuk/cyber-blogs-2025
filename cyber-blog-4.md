## Overview
Threat actors have been actively targeting Microsoft 365 and Gmail accounts with an adversary-in-the-middle (AiTM) phishing kit designed to bypass multifactor authentication (MFA) by intercepting communication between users and the legitimate services, capturing session cookies from authenticated sessions. The ready-to-use phishing campaigns, typically distribute phishing pages, as many security professionals would expect, through URL redirects and QR codes embedded in email attachments or bodies. The pages often employ themes related to human resources, finance, or security, leveraging fear-based lures to persuade targets to follow the steps leading to credential sharing and MFA challenge resolution. There have been decoys observed mimicking DocuSign, Microsoft, Adobe, and others.

Although active since 2023, the Tycoon 2FA phishing kit has made stealthy improvements. Trustwave has described three major changes implemented to bypass detections, that defenders should be mindful of: 
- Invisible Unicode Characters: Tycoon 2FA employs hidden Unicode characters to disguise its JavaScript code. This method renders the payload undetectable to human eyes and complicates static analysis 
- Custom CAPTCHA: Instead of relying on third-party CAPTCHA services, like Cloudflare Turnstile, Tycoon 2FA now opts for a custom CAPTCHA created with HTML5 
- Anti-Debugging Scripts: The kit includes aggressive anti-debugging measures such as detecting browser automations, preventing inspection by disabling right clicks, and redirection if analysis is expected

### Why it matters:
Although each technique on its own may not be revolutionary, their combined application can significantly impact detection and response efforts. The HTML5 based visuals increase engagement and the appearance of credibility amongst end-users, and the obfuscation and anti-debugging features defer detection and complicate analysis for defenders and researchers. 
This evolution raises concerns about the effectiveness of current MFA implementations, and the contemplation of additional layers of authentication beyond MFA, such as biometric verification or hardware tokens. This also highlights the need for continuous user education, regularly training employees on recognizing phishing attempts, especially those involving QR codes and URL redirects.

### References
- [BleepingComputer: Tycoon2FA Phishing Kit Targets Microsoft 365 with New Tricks](https://www.bleepingcomputer.com/news/security/tycoon2fa-phishing-kit-targets-microsoft-365-with-new-tricks/)
- [Trustwave SpiderLabs: Tycoon2FA — New Evasion Technique Spotted in 2025](https://www.trustwave.com/en-us/resources/blogs/spiderlabs-blog/tycoon2fa-new-evasion-technique-for-2025/)
- [ITSecurityNewsBox: Tycoon2FA Phishing Kit Rollout with Significant Updates (April 2025)](https://itsecuritynewsbox.com/index.php/2025/04/14/tycoon2fa-phishing-kit-rolled-out-significant-updates/)
