# DNS & HTTP/HTTPS Deep Dive (summary)

## DNS (Domain Name System)
- Purpose: translate domain names to IP addresses.
- Record types: A (IPv4), AAAA (IPv6), CNAME, MX, TXT, NS, SOA.
- Resolution flow: Resolver -> Recursive resolver -> Authoritative nameserver.
- Security: DNSSEC adds signatures to prevent spoofing.

## HTTP
- Stateless, application-layer protocol for the web.
- Methods: GET, POST, PUT, DELETE, HEAD, OPTIONS.
- Status codes: 2xx success, 3xx redirect, 4xx client error, 5xx server error.
- Headers: Host, User-Agent, Cookie, Content-Type, Authorization.

## HTTPS & TLS/SSL (overview)
- HTTPS = HTTP over TLS. TLS provides encryption, integrity, and auth.
- TLS handshake (simplified): ClientHello -> ServerHello -> Certificate -> Key exchange -> Finished.
- Certificates: X.509 certs signed by CAs; include public key, subject, validity.
- Cipher suites: specify key exchange, auth, symmetric cipher, MAC (e.g., ECDHE-RSA-AES128-GCM-SHA256).
- TLS versions: TLS 1.2, TLS 1.3 (preferred). SSLv2/3 deprecated.

## Practical tips
- Use `openssl s_client -connect host:443 -servername host` to inspect certs.
- Check HSTS, certificate chain, and OCSP/CRL for revocation.
