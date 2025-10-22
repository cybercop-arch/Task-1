# Attack Vectors — How attackers reach targets

## Social Engineering
- Definition: Manipulating people to give up confidential information or perform actions.
- Examples: Phishing emails, pretexting (impersonation), baiting (USB drops), quid pro quo.
- Mitigations: Security awareness training, verification procedures, strict policies for sensitive actions, phishing simulations.

## Wireless Attacks
- Definition: Exploiting wireless networks (Wi‑Fi, Bluetooth) to intercept, impersonate, or inject traffic.
- Common attacks: Rogue access points, evil twin, WPA2/3 vulnerabilities (KRACK historically), WPA‑PSK cracking, deauthentication attacks.
- Mitigations: Use enterprise-grade authentication (WPA2-Enterprise/EAP), strong encryption, disable WPS, monitor wireless environment, use network segmentation and VPN for sensitive access.

## Insider Threats
- Definition: Threats originating from employees, contractors, or partners with legitimate access.
- Types: Malicious insiders, negligent insiders, compromised accounts.
- Mitigations: Principle of least privilege, role-based access, logging and audit trails, user behavior analytics (UBA), separation of duties, background checks, offboarding procedures.

## Additional vectors (brief)
- Supply chain attacks: Compromised software or third-party services.
- Physical attacks: Theft of devices, unauthorized physical access.
- API abuse: Broken access controls, insecure endpoints.

## Defending vectors
- Combine technical controls (auth, encryption, monitoring) with people/process controls (training, policies, audits).
- Regularly test (penetration testing, red teaming, tabletop exercises).
