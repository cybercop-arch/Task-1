# Threat Types — Overview & Mitigations

This file covers common threat types and practical mitigations.

## 1. Phishing
- Description: Deceptive messages (email, SMS) that trick users into revealing credentials or running malware.
- Indicators: Unexpected links, mismatched URLs, urgency, spoofed sender addresses.
- Mitigations: User training, email filtering, DMARC/DKIM/SPF, MFA, link and attachment sandboxing.

## 2. Malware
- Description: Malicious software (viruses, worms, trojans, spyware, rootkits).
- Delivery: Drive-by downloads, attachments, USBs, compromised installers.
- Mitigations: Endpoint protection (EDR), patching, application allowlisting, least privilege, network segmentation.

## 3. Distributed Denial of Service (DDoS)
- Description: Overwhelm resources using large volumes of traffic or resource exhaustion.
- Types: Volumetric, protocol, application-layer attacks.
- Mitigations: Rate-limiting, CDNs, upstream filtering, autoscaling, DDoS protection services (Cloudflare, AWS Shield).

## 4. SQL Injection (SQLi)
- Description: Injection of malicious SQL through unsanitized inputs allowing DB read/modification.
- Indicators: Unexpected database errors, unusual query patterns.
- Mitigations: Parameterized queries / prepared statements, ORM usage, input validation, least privilege DB accounts, WAF rules.

## 5. Brute Force
- Description: Repeated attempts to guess credentials (passwords, SSH keys).
- Mitigations: Account lockout policies, rate limiting, MFA, strong password policies, fail2ban/automation.

## 6. Ransomware
- Description: Malware that encrypts files and demands payment for decryption.
- Attack chain: Initial access (phishing/credentials) -> lateral movement -> encryption -> demands.
- Mitigations: Offline backups, EDR, network segmentation, patching, MFA, least privilege, rapid incident response.

## General advice
- Apply defense-in-depth: multiple overlapping controls.
- Monitor logs and alerts and have an incident response plan.
