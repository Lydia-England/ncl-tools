# Scanning and Reconnaissance

## Command Line Scanning and Reconnaissance Tools
- [Nmap](/#Nmap)
- `nc` —
- `amap` — 
- `dirbust/dirb/dir` —
- [Dirbuster](https://www.kali.org/tools/dirbuster/) —
- `telnet` —
- [`smtp-user-enum`](https://pentestmonkey.net/tools/user-enumeration/smtp-user-enum) — Username guessing tool primarily for use against the default SMTP service.
  - [Linux username wordlist](https://github.com/rapid7/metasploit-framework/blob/master/data/wordlists/unix_users.txt)

## Graphical Scanning and Reconnaissance Tools
- [Zenmap](https://nmap.org/zenmap/) — A graphical user interface for Nmap.

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
- Stealth scan:
  ```bash
  nmap -sS scanme.nmap.org
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
