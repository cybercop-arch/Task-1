# Networking Commands, OSI Model & TCP/IP Suite

## Useful Networking Commands
- `ifconfig` or `ip a` — show interfaces and IP addresses
- `ping -c 4 host` — basic reachability
- `netstat -tulnp` or `ss -tulnp` — listening sockets and processes
- `traceroute host` — path to host (replace with `tracert` on Windows)
- `nslookup host` / `dig host` — DNS queries
- `route -n` or `ip r` — routing table

## OSI Model — 7 Layers (brief)
7. Application — user-facing apps (HTTP, SMTP, DNS)
6. Presentation — data representation, encryption (TLS)
5. Session — sessions, connections
4. Transport — end-to-end (TCP/UDP)
3. Network — IP addressing/routing (IPv4/IPv6)
2. Data Link — MAC addresses, switches (Ethernet)
1. Physical — cables, radio, physical medium

## TCP/IP Protocol Suite (4 layers mapping)
- Application (HTTP, DNS, SMTP, FTP)
- Transport (TCP, UDP)
- Internet (IP, ICMP)
- Link (Ethernet, Wi‑Fi)

## Notes
- OSI is conceptual; TCP/IP is the practical stack used on the internet.
