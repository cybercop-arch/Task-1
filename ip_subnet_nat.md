# IP Addressing, Subnetting & NAT

## IP Addressing
- IPv4: dotted decimal (e.g., 192.168.1.10). IPv6: hexcolon notation.
- Classes (historical): A/B/C; modern use CIDR.

## Subnetting (CIDR)
- CIDR notation: 192.168.1.0/24 means netmask 255.255.255.0 (256 addresses).
- Calculate hosts: host bits = 32 - prefix; hosts = 2^host_bits - 2 (network & broadcast).
- Example: /24 -> 254 hosts; /30 -> 2 hosts.

## NAT (Network Address Translation)
- Purpose: map private IPs to a public IP, conserve IPv4 addresses, provide basic isolation.
- Types: SNAT (source NAT), DNAT (destination NAT), PAT (port address translation).
- Home router uses PAT to map multiple internal hosts to one public IP.

## Quick subnet examples
- /25 -> 128 addresses (126 hosts)
- /26 -> 64 addresses (62 hosts)
- /29 -> 8 addresses (6 hosts)
