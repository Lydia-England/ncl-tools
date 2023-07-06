# NCL Tools and Resources
The [National Cyber League (NCL)](https://nationalcyberleague.org/) is a bi-annual, virtual cybersecurity competition for high school and undergraduate students. 
This is a non-exhaustive list of tools I've found useful during the competition or that were recommended to me.

## Categories
---
- [Open Source Intelligence](/#Open-Source-Intelligence)
- [Cryptography](/#Cryptography)
- [Password Cracking](/#Password-Cracking)
- [Log Analysis](/#Log-Analysis)
- [Network Traffic Analysis](/#Network-Traffic-Analysis)
- [Forensics](/#Forensics)
- [Wireless Access Exploitation](/#Wireless-Access-Exploitation)
- [Scanning and Recon](/#Scanning-and-Recon)
- [Web Application Exploitation](/#Web-Application-Exploitation)
- [Enumeration and Exploitation](/#Enumeration-and-Exploitation)

## Appendix
---
- [Kali Linux](#/Kali-Linux)
- [Python Virtual Environment](#/Python-Virtual-Environment)
- [Vim](#/Vim)
- [Additional Resources](#/Additional-Resources)


## Open Source Intelligence
---
### OSINT Web Resources
- [exif.regex.info](exif.regex.info) — Metadata viewer
- [Google Reverse Image Search](images.google.com) — Reverse image search
- [Github](github.com) — Code repository (lol)
- [Shodan](shodan.io) — Search engine for web services
- [Greynoise](greynoise.io) — IP reputation search
- [Maxmind](maxmind.com) — GeoIP lookup
- [web.archive.org](web.archive.org) — The Internet archive
- [Latitude and Longitude converter](https://www.fcc.gov/media/radio/dms-decimal) — Degrees Minutes Seconds to/from Decimal Degrees
- [Cert Logik](https://certlogik.com/decoder/) — CSR Decoder and Certificate Decoder
- [Geocode 3 Word System](https://what3words.com/royal.grass.prep) — Geocode system labeling every 3 meter square of the world with a unique 3-word combination.
- [Online Exiftool](https://exif.tools/) — Online File Metadata Extraction
### Command Line OSINT Tools
- [ExifTool](https://exiftool.org/) — Meta information reader/writer
  - [File types and meta information formats supported by ExifTool](https://github.com/exiftool/exiftool)
  - `exiftool <filename>`
### OSINT Misc. Information and Resources
- [50 Common Ports You Should Know](https://www.geeksforgeeks.org/50-common-ports-you-should-know/#)
- [Service Name and Transport Protocol Port Number Registry](https://www.iana.org/assignments/service-names-port-numbers/service-names-port-numbers.xhtml) — IANA
- [Google Dork Cheatsheet](https://gist.github.com/sundowndev/283efaddbcf896ab405488330d1bbc06)
- [List of DNS Record Types](https://en.wikipedia.org/wiki/List_of_DNS_record_types)
- [Google Hacking Database](https://www.exploit-db.com/google-hacking-database)


## Cryptography
---
### Online Cipher Identification and Decryption Tools
- [dcode](https://www.dcode.fr/cipher-identifier) — Cipher Identifier
  - [Caesar Cipher](https://www.dcode.fr/caesar-cipher)
  - [Morse Code Translator](https://morsedecoder.com/)
  - [Letter Number Code](https://www.dcode.fr/letter-number-cipher)
  - [Braille Alphabet](https://www.dcode.fr/braille-alphabet)
  - [Atbash Cipher](https://www.dcode.fr/atbash-cipher)
- [cryptii](https://cryptii.com/) — Modular conversion, encoding, and encryption online.
- [CacheSleuth](https://www.cachesleuth.com/multidecoder/) — Mutli Decoder
- Number Bases Converters and Translators
  - [Base64 Converter](https://www.base64decode.org/)
  - [Hex to ASCII Converter](https://www.rapidtables.com/convert/number/hex-to-ascii.html)
  - [Octal to Text Converter](https://www.browserling.com/tools/octal-to-text)
- [CodeBeautify](https://codebeautify.org/) — Code Formatter, Decode, Convert
  - [ZLib Decompress Online](https://codebeautify.org/zlib-decompress-online)
  - [Number System Converter](https://codebeautify.org/all-number-converter)
  - [JSON Beautifier, Viewer](https://codebeautify.org/jsonviewer), [JSON Validator](https://codebeautify.org/jsonvalidator), [JSON Cheat Sheet](https://codebeautify.org/json-cheat-sheet)
  - [HTML Viewer](https://codebeautify.org/htmlviewer)
  - [Image to Base64](https://codebeautify.org/image-to-base64-converter) / [Base64 to Image](https://codebeautify.org/base64-to-image-converter)
  - [HEX to Decimal](https://codebeautify.org/hex-decimal-converter) / [Decimal to Hex](https://codebeautify.org/decimal-hex-converter)
  - [Binary to Text](https://codebeautify.org/binary-to-text), [Binary to Decimal](https://codebeautify.org/binary-decimal-converter)
  - [ASCII to Text](https://codebeautify.org/ascii-to-text)
  - [Encryption/Decryption](https://codebeautify.org/encrypt-decrypt)
  - ...and more
### Online Steganography Tools
- [StegOnline](https://stegonline.georgeom.net/upload) — Online Steg Decoder
- [FotoForensics](https://fotoforensics.com/analysis.php?id=b4727b6206fb898a6ae76ea14d8d6ae4fc623752.110213)
  - Supported formats: JPEG, PNG, WebP, HEIC, and AVIF.
  - The "Hidden Pixels" analysis option is particularly useful.
- [Online Exiftool](https://exif.tools/) — Online File Metadata Extraction
### Online RSA Decryption Tools
- [Integer Factorization Calculator](https://www.alpertron.com.ar/ECM.HTM)
### Command Line Cryptography Tools
- [RsaCtfTool](https://github.com/RsaCtfTool/RsaCtfTool) — Uncipher data from weak public keys and attempt to recover the corresponding private key.
-   [ExifTool](https://exiftool.org/) — Meta information reader/writer
  - [File types and meta information formats supported by ExifTool](https://github.com/exiftool/exiftool)
  - `exiftool <filename>`
- [OpenSSL](https://www.openssl.org/) — Command line program for using cryptography functions of OpenSSL's crypto library from the shell.
  - [`openssl` Program Docs](https://www.openssl.org/docs/manmaster/man1/openssl.html#SYNOPSIS)
### Cryptography Software
- [DIIT](https://diit.sourceforge.net/) — Digital Invisible Ink Toolkit
### Additional Resources
- [Chart to Identify Number Bases](https://cryptokait.com/2020/05/27/summer-camp-2020-numerical-cryptography/)



## Password Cracking
---
### Online Password Cracking Tools
--- 
- [MD5 Hash Generator](https://www.md5hashgenerator.com/)
- [SHA256 Hash Generator](https://emn178.github.io/online-tools/sha256.html)
- [CrackStation](https://crackstation.net/) — Online Password Hash Cracking
### Command Line Tools
--- 
- [`hash-identifier`](https://www.kali.org/tools/hash-identifier/)
- `hashcat` (more below)
- [`fcrackzip`](https://www.kali.org/tools/fcrackzip/) — Zip Password Cracker
- [John the Ripper](https://www.openwall.com/john/) — Password Cracker
- [Ophcrack](https://ophcrack.sourceforge.io/) — Windows password cracker based on rainbow tables.
### Hashcat
---
- With known format SKY-ABCD-####: `hashcat -m 0 -a 3 hashes.txt SKY-ABCD-?d?d?d?d`
  - `-m 0` for MD5 hashes.
  - `-a 3` for brute force and mask attack mode.
- Using the rockyou wordlist: `hashcat -m 0 -a 0 hashes.txt rockyou.txt`
- [Hybrid attacks](https://hashcat.net/wiki/doku.php?id=hybrid_attack)
- [Rule-based attacks](https://hashcat.net/wiki/doku.php?id=rule_based_attack)
- [Extracting WPA and WPA2 hashes from PCAPs for use with hashcat](https://hashcat.net/wiki/doku.php?id=hccapx)
Hashcat example hashes and associated codes found [here](https://hashcat.net/wiki/doku.php?id=example_hashes).





## Log Analysis
---
### Command Line Log Analysis Tools
- `cut` extracts column(s) from a file or text stream. Columns must be delineated by a consistent character. 
  - `cut example.txt -d , -f 2` prints the second column from example.txt where a comma is used to separate each column.
- `sort` sorts the lines from a file or text stream.
  - `sort example.txt` prints the sorted output of the lines from example.txt.
  - `sort -n example.txt` uses numberical value to sort.
  - `sort -b example.txt` ignores blanks at the start of the line.
  - `sort -r example.txt` reverses the sorting order.
  - `-k` flag is useful for sorting databases.
- `uniq` prints the result of removing any duplicate lines from a file or text stream.
  - `uniq example.txt` prints the result of removing any duplicate lines from example.txt.
  - Usually use this after using `sort`; it only removes adjacent duplicate lines.
- `grep` "Global Regular Expression Print" searches for text that matches a specific pattern.
  - `grep match example.txt` prints lines that contain the text "match" in example.txt.
  - grep IP address: `grep -E '[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}' example.txt`
  - grep only valid IP address: `grep -E '^((25[0-5]|2[0-4][0-9]|[1]?[1-9][0-9]?).){3}(25[0-5]|2[0-4][0-9]|[1]?[1-9]?[0-9])$' example.txt`
    - `ping` to remove leading zeros.
- `wc` "Word Count" gets a line count (followed by a word count and a byte count) of a file or text stream.
  - `wc example.txt` prints the number of lines, words, bytes in example.txt.
  - `-l` flag to print number of lines only.
  - `-c` flag to print number of bytes only.
  - `-w` flag to print number of words only. A word is defined as a string of characters delimited by spaces, tabs, or newline characters.
- `awk` is a tool used to manipulate data. It can be used to extract specific columns from data.
  - `cat example.txt | awk '{print #2}'` prints the second column in example.txt.
- `tail` prints the last several lines of a file.
  - `tail example.txt` prints the last lines of example.txt.
### Creating Programs to do Log Analysis
- `.json` File, Python analysis:
  - *Find unique IPs, unique signatures, most popular category, total bytes sent, category of non TCP traffic*
```python
import json
f = open('filename.json')
data = json.load(f)
for entry in data:
  print(entry['dest_ip'])
  print(entry['alert']['signature'])
  print(entry['alert']['category'])
  if 'xx.xx.xx.xx' == entry['dest_ip']:
    total_bytes += entry['flow']['bytes_toserver']
  if 'xx.xx.xx.xx' == entry['src_ip']:
    total_bytes += entry['flow']['bytes_toserver']
  if 'TCP' not in entry['proto']:
    print(entry['alert']['category'])
```



## Network Traffic Analysis
---
### Command Line Network Traffic Analysis Tools
- `TCPDump`
- `Wireshark`



## Forensics
---
### Online Forensics Tools
- [Online Hex Editor](https://hexed.it/)
- [FotoForensics](https://fotoforensics.com/analysis.php?id=b4727b6206fb898a6ae76ea14d8d6ae4fc623752.110213)
  - Supported formats: JPEG, PNG, WebP, HEIC, and AVIF.
  - The "Hidden Pixels" analysis option is particularly useful.
### Command Line Forensics Tools
- `file`
- `binwalk`
- `exiftool`
- `exif`
- `xxd` — dump file in hex format.
- `strings`
- `steghide`
- `foremost`
- `zsteg`
  - `zsteg -a` runs every detection method on the given file.
  - `zsteg -E` extracts data with the given payload.
- `stegsolve`
- `fft` (Fast Fourier Transform)
- `stegoveritas` — carve and extract.
- [`scalpel`](https://www.kali.org/tools/scalpel/#scalpel) — fast file carver that reads database of header and footer definitions and extracts matching files from a set of image files or raw device files.
- `unrar`
- `unzip filename.docx -d out` to unzip .docx files to see what's inside.
### Graphical Forensics Tools
- [Autopsy Forensic Browser](https://www.kali.org/tools/autopsy/)
  

## Wireless Access Exploitation
---
### Command Line Wireless Access Exploitation Tools
- [Aircrack-ng Suite](https://aircrack-ng.org/documentation.html)
  - `aircrack-ng`
- `Airplay`
- [Wireshark](https://www.wireshark.org/)



## Scanning and Reconnaissance
---
### Command Line Scanning and Reconnaissance Tools
- [Nmap](https://www.kali.org/tools/nmap/) — "Network Mapper", a network scanning tool.
  - Ping scan: `nmap -sp 192.168.1.1/24`
  - Scan a single host: `nmap scanme.nmap.org`
  - Stealth scan: `nmap -sS scanme.nmap.org`
  - Version scan: `nmap -sV scanme.nmap.org`
  - OS scanning: `nmap -sV scanme.nmap.org`
  - Aggressive scan: `nmap -A scanme.nmap.org`
  - Scanning multiple hosts (several approaches)
  - Port scanning: `nmap -p 973 192.164.0.1`
  - Port scanning for information about a particular type of connection (here, TCP connection): `nmap -p T:7777, 973 192.164.0.1`
  - Range of ports: `nmap -p 76-973 192.164.0.1`
  - Top Ports: `nmap --top-ports 10 scanme.nmap.org`
  - Scanning from a file with a list of IP addresses: `nmap -iL /input_ips.txt`
- `nc`
- `amap`
- `dirbust/dirb/dir`
- [Dirbuster](https://www.kali.org/tools/dirbuster/)
- `telnet`
- [`smtp-user-enum`](https://pentestmonkey.net/tools/user-enumeration/smtp-user-enum) — Username guessing tool primarily for use against the default SMTP service.
  - [Linux username wordlist](https://github.com/rapid7/metasploit-framework/blob/master/data/wordlists/unix_users.txt)
### Graphical Scanning and Reconnaissance Tools
- [Zenmap](https://nmap.org/zenmap/) — a graphical user interface for Nmap.


## Web Application Exploitation
---
### Command Line Web Application Exploitation Tools
- `SQLMap`
- `wpscan`
- `burpsuite`
- `hackbar`
- `editthiscookie`
- `firebug`




## Enumeration and Exploitation
---
### Command Line Enumeration and Exploitation Tools
- `uncompyle6`



# Appendix

## Kali Linux
--- 
- [Kali Tools Documentation](https://www.kali.org/tools/)


## Python Virtual Environment
--- 
Python documentation on how to create a virtual environment with `venv` can be found [here](https://docs.python.org/3/library/venv.html).
Information on installing packages with `pip` in a virtual environment can be found [here](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/).


## Vim
---



## Additional Resources
--- 





