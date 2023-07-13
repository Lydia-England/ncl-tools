# Scanning and Reconnaissance

## Online Scanning and Reconnaissance Tools
- [ICANN registration data lookup tool](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwig88e15oWAAxVgIjQIHZdXCMMQFnoECA8QAQ&url=https%3A%2F%2Flookup.icann.org%2F&usg=AOvVaw0AnKZxWMO4k3aXI_DKuq0f&opi=89978449) — WHOIS search tool
- [Autonomous System Lookup (AS/ASN/IP)](https://hackertarget.com/as-ip-lookup/)
- [Website to IP Lookup](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwiA3I6ZjIeAAxUZO0QIHXkSBSEQFnoECA0QAQ&url=https%3A%2F%2Fwww.nslookup.io%2Fwebsite-to-ip-lookup%2F&usg=AOvVaw169x1zRLKwwWjrdHJwkaCZ&opi=89978449)

## Scanning and Reconnaissance Tools
- [Dirbuster](https://www.kali.org/tools/dirbuster/) —
- dirb
  - Brute force HTTP(s) directories and files.
- nikto
- wfuzz
- cewl (creating wordlist from webpage)
- [`smtp-user-enum`](https://pentestmonkey.net/tools/user-enumeration/smtp-user-enum) — Username guessing tool primarily for use against the default SMTP service.
  - [Linux username wordlist](https://github.com/rapid7/metasploit-framework/blob/master/data/wordlists/unix_users.txt)
- `wget`

- [Zenmap](https://nmap.org/zenmap/) — A graphical user interface for Nmap.




## Nslookup
- Interactive or non-interactive modes.

Syntax:
```bash
nslookup [options] [website or IP address]
```

Running without options should return the IP address associated with a website (or website associated with IP address).

Nslookup options:
- `-domain=[domain name]` option to change the default DNS name.
- `-debug` option to show debugging information.
- `-timeout=[seconds]` option to specify the time allowed for the server to respond.
- `-port=[port number]` option to specify the port for queries. Default port number is 53.
- `-type=a` to view information about the DNS A address records.
- `-type=any` to view all available records.
- `-type=hinfo` to view hardware-related information about the host.
- `-type=mx` to view Mail Exchange (MX) server information.
- `-type=ns` to view Name Server (NS) records.
- `-type=ptr` to view Pointer records. Used in reverse DNS lookups.
- `-type=soa` to view Start of Authority records.

How to use nslookup:
- View NS records for a domain:
  ```bash
  nslookup -type=ns [domain name]
  ```
- View MX (Mail Exchange server data) records for a domain:
  ```bash
  nslookup -type=mx [domain name]
  ```
- Perform a reverse DNS lookup (find domain name associated with IP address): 
  ```bash
  nslookup [domain name]
  ```
- View all available logs: 
  ```bash
  nslookup -type=any [domain name]
  ```


## Dig
[Dig documentation found here](https://linux.die.net/man/1/dig).
Dig (domain information groper) is a flexible tool for interrogating DNS name servers.
Basic usage looks like the following:
```bash 
dig @server name type
```
where `server` is the name or IP address of the name server to query. 
This can be an IPv4 address in dotted-decimal notation or an IPv6 address in colon-delimited notation.
`name` is the name of the resource record that is to be looked up.
`type` indicates what type of query is required.
Valid query types include: `A`, `AAAA`, `MX`, `SIG`, `SOA`, `TXT`, etc.



## Nmap
[Nmap](https://www.kali.org/tools/nmap/) — "Network Mapper", a network scanning tool.
- Ping scan:
  ```bash
  nmap -sp 192.168.1.1/24
  ```
- No ping (skip host discovery stage) 
  ```bash
  nmap -Pn 192.168.1.1/24
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


## The Heartbleed Bug
[The Heartbleed Bug](https://heartbleed.com/) is a vulnerability in the OpenSSL cryptographic software library. 

Investigate if an https page is vulnerable to heartbleed:
```bash
sudo sslscan <ip address>:443
```
Or with an nmap script:
```bash
nmap -sV --script=ssl-heartbleed <ip address>
```

Exploit Heartbleed vulnerability:
- Module in burp suite. 
- Metasploit module.
```bash
use auxiliary/scanner/ssl/openssl_heartbleed
set RHOSTS <ip address>
set verbose true
run
```




## HTTP response status codes
- Informational response (100-199)
- Successful response (200-299)
- Redirection message (300-399)
- Client error response (400-499)
  - `403 Forbidden`: The client doesn't have rights to access the content; it's unauthorized, so the server is refusing to give the requested resource. Unlike `401 Unauthorized`, the client's identity is known to the server.
- Server error response (500-599)


## DNS Record Types
- A records resolve to IPv4 addresses.
- AAAA records resolve to IPv6 addresses.
- CNAME records resolve to another domain name (like a subdomain).
- MX records resolve to the address of the servers that handle the email for the domain you are querying.
- TXT records are free text fields where any text-based data can be stored.


## SSH Key Pairs
SSH employs public key cryptography (a.k.a. asymmetric cryptography), which requires two separate keys: one private key, and one public key.
Together, the public and private key compose a key pair. 
In SSH, the public key cryptography is used in both directions (client to server and server to client), so two key pairs are used. 
One key pair is the host (server) key; one is the user (client) key.
[This article](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwiU2L_lgoqAAxUOHzQIHQojDF8QFnoECAgQAQ&url=https%3A%2F%2Fdocs.oracle.com%2Fen%2Fcloud%2Fcloud-at-customer%2Focc-get-started%2Fgenerate-ssh-key-pair.html&usg=AOvVaw0-nDex6Sg1StUuJy8sZon5&opi=89978449) details how to generate an SSH Key Pair. 



## Acronyms and Definitions
- ASN: Autonomous System Number
- AS: Autonomous System
- DNS: Domain Name System
- IP: Internet Protocol
- RIR: Regional Internet Registry
- SOA: Start of Authority. DNS SOA record used to designate the primary name server and administrator responsible for a zone.
- SSL: Secure Sockets Layer
  - CN: SSL Certificate Common Name (a.k.a. Fully Qualified Domain Name (FQDN))
- TLD: Top-Level Domain
- TTL: Time to live (also known as "hop limit") - specifies how long a DNS record should be cached for.
