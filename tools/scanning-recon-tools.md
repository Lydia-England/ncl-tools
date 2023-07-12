# Scanning and Reconnaissance

## Online Scanning and Reconnaissance Tools
- [ICANN registration data lookup tool](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwig88e15oWAAxVgIjQIHZdXCMMQFnoECA8QAQ&url=https%3A%2F%2Flookup.icann.org%2F&usg=AOvVaw0AnKZxWMO4k3aXI_DKuq0f&opi=89978449) — WHOIS search tool
- [Autonomous System Lookup (AS/ASN/IP)](https://hackertarget.com/as-ip-lookup/)
- [Website to IP Lookup](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwiA3I6ZjIeAAxUZO0QIHXkSBSEQFnoECA0QAQ&url=https%3A%2F%2Fwww.nslookup.io%2Fwebsite-to-ip-lookup%2F&usg=AOvVaw169x1zRLKwwWjrdHJwkaCZ&opi=89978449)

## Command Line Scanning and Reconnaissance Tools
- [Nmap](/#Nmap)
- [Nslookup](/#Nslookup)
- `nc` —
- `amap` — 
- `dirbust/dirb/dir` —
- [Dirbuster](https://www.kali.org/tools/dirbuster/) —
- `telnet` —
- [`smtp-user-enum`](https://pentestmonkey.net/tools/user-enumeration/smtp-user-enum) — Username guessing tool primarily for use against the default SMTP service.
  - [Linux username wordlist](https://github.com/rapid7/metasploit-framework/blob/master/data/wordlists/unix_users.txt)
- `wget`

## Graphical Scanning and Reconnaissance Tools
- [Zenmap](https://nmap.org/zenmap/) — A graphical user interface for Nmap.

## Nslookup
- Interactive or non-interactive modes.
Syntax:
```bash
nslookup [options] [website or IP address]
```
- `nslookup <website>` to find IP address of a website.
Nslookup options:
- `-domain=[domain name]` option to change the default DNS name.
- `-port=[port number]` option to specify the port for queries. Default port number is 53.
- `-type=a` to view information about the DNS A address records.
- `-type=any` to view all available records.
- `-type=hinfo` to view hardware-related information about the host.
- `-type=mx` to view Mail Exchange server information.
- `-type=ns` to view Name Server (NS) records.
- `-type=ptr` to view Pointer records. Used in reverse DNS lookups.
- `-type=soa` to view Start of Authority records.


## Nmap
[Nmap](https://www.kali.org/tools/nmap/) — "Network Mapper", a network scanning tool.
- Ping scan:
  ```bash
  nmap -sp 192.168.1.1/24
  ```
- Scan a single host:
  ```bash
  nmap scanme.nmap.org
  ```
- Stealth scan (TCP SYN scan):
  ```bash
  nmap -sS scanme.nmap.org
  ```
- UDP scan:
  ```bash
  nmap -sU scanme.nmap.org
  ```
- Version scan:
  ```bash
  nmap -sV scanme.nmap.org
  ```
- OS scanning:
  ```bash
  nmap -sV scanme.nmap.org
  ```
- Aggressive scan:
  ```bash
  nmap -A scanme.nmap.org
  ```
- Scanning multiple hosts (several approaches)
- Port scanning:
  ```bash
  nmap -p 973 192.164.0.1
  ```
- Port scanning for information about a particular type of connection (here, TCP connection):
  ```bash
  nmap -p T:7777, 973 192.164.0.1
  ```
- More options: 
  - `-S` to spoof an IP address
  - `-6` to conduct an IPv6 scan


## OpenSSL
- [OpenSSL Documentation](https://www.openssl.org/docs/manmaster/man1/pkcs7.html)
- Check SSL certificate expiration date
  ```bash
  cat cert.cer | openssl x509 -noout -enddate
  ```

## HTTP response status codes
- Informational response (100-199)
- Successful response (200-299)
- Redirection message (300-399)
- Client error response (400-499)
  - `403 Forbidden`: The client doesn't have rights to access the content; it's unauthorized, so the server is refusing to give the requested resource. Unlike `401 Unauthorized`, the client's identity is known to the server.
- Server error response (500-599)


## Acronyms and Definitions
- ASN: Autonomous System Number
- AS: Autonomous System
- DNS: Domain Name System
- IP: Internet Protocol
- RIR: Regional Internet Registry
- SSL: Secure Sockets Layer
  - CN: SSL Certificate Common Name (a.k.a. Fully Qualified Domain Name (FQDN))
