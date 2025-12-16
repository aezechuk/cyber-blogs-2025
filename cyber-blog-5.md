### Overview
A new type of remote access trojan (RAT), deemed ResolverRAT, has been discovered targeting healthcare and pharmaceutical sectors globally. This malware's main goal is to follow instructions from its command-and-control server and steal sensitive data from infected systems. Although ResolverRAT shares some traits with malware campaigns spreading Lumma and Rhadamanthys infostealers, it has been has classified in a malware family of its own due to some unique variations in architecture and layered evasion techniques

Initial access is gained through phishing emails that look like legal or copyright violation notices, written in the recipient's localized language to appear more credible. When the victim clicks the link, the malware uses a technique to load a malicious file alongside a legitimate one, such as "hpreader.exe", starting the infection. Morphisec Labs identified and disclosed many technical details about what makes ResolverRat harder to spot and stop, some are listed below:

- Reflective DLL Injection: ResolverRAT uses reflective DLL injection to load malicious code directly into memory, bypassing disk-based detection methods, by avoiding writing anything to disk. 
- .NET ResourceResolver Hijacking: The malware hijacks the .NET ResourceResolve event to load malicious assemblies without triggering suspicious API calls that may trigger detections, this allows ResolverRAT to operate within managed memory. 
- Custom certificate validation process: During SSL/TLS handshakes, ResolverRat uses pre-embedded X509 certificates instead of the system's root authorities. This parallel trust system allows the malware to establish secure connections without triggering alerts from traditional security mechanisms, blending its communications into regular network traffic.

### Why it matters: 
ResolverRAT poses a significant threat, especially to healthcare and pharmaceutical organizations, making it very difficult to detect sensitive data flowing out over the wire. Researchers are yet to attribute ResolverRat to any particular threat actor but the sophistication of execution lends to threat actors of the highest level. Enhanced email security, endpoint detection with behavioral analysis, and regular auditing of systems for unusual memory activity are more important than ever. All software, especially those used for document handling and PDF readers, should be regularly updated to patch vulnerabilities. As always remain vigilant in educating end users on phishing tactics, especially those with urgent or fear-based messages.

### References
- [InfoSecurity Magazine: Malware “ResolverRat” Targets Healthcare and Pharma](https://www.infosecurity-magazine.com/news/malware-resolverrat-targets/)
- [BleepingComputer: New ResolverRat Malware Targets Pharma and Healthcare Organizations Worldwide](https://www.bleepingcomputer.com/news/security/new-resolverrat-malware-targets-pharma-and-healthcare-orgs-worldwide/)
- [Morphisec Blog: New Malware Variant Identified — ResolverRat Enters the Maze](https://www.morphisec.com/blog/new-malware-variant-identified-resolverrat-enters-the-maze/)
