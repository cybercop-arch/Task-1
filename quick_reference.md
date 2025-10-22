# Quick Reference — Interview / Revision Bullets

## CIA Triad
- Confidentiality: Encryption, access control, MFA.
- Integrity: Hashes, digital signatures, secure logging.
- Availability: Backups, redundancy, DDoS protections.

## Threats
- Phishing -> user education + email auth (DMARC/DKIM/SPF) + MFA.
- Malware -> EDR + patching + app allowlisting.
- DDoS -> CDN, rate-limiting, autoscale.
- SQLi -> prepared statements, input validation.
- Brute Force -> rate-limit, lockouts, MFA.
- Ransomware -> offline backups, segmentation, EDR.

## Attack Vectors
- Social engineering -> policies + training + verification checks.
- Wireless -> WPA2-Enterprise, monitor, VPN.
- Insider -> least privilege, auditing, UBA.

## Commands & tools to know
- nmap, wireshark/tcpdump, burpsuite, sqlmap, metasploit (for testing in lab), splunk/ELK (for log analysis).


## Additional Topics
- File system navigation: `pwd`, `ls`, `cd`, `mkdir`, `rm -rf`.
- Permissions: `chmod`, `chown`, `stat`.
- Package management: `apt`, `dpkg`.
- Networking: `ifconfig`/`ip a`, `ping`, `netstat`/`ss`, `traceroute`, `dig`/`nslookup`.
- OSI model & TCP/IP layers — know key protocols per layer.
- DNS, HTTP/HTTPS basics and TLS inspection with `openssl s_client`.
- Subnetting: CIDR notation and host calculations.
- Crypto: Symmetric vs Asymmetric, hashing (SHA256), certificates, OpenSSL examples.
- Tools: wireshark, nmap, burp-suite, netcat.
