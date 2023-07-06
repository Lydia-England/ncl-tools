# NCL Tools and Resources
The [National Cyber League (NCL)](https://nationalcyberleague.org/) is a bi-annual, virtual cybersecurity competition for high school and undergraduate students. 
This is a non-exhaustive list of tools I've found useful during the competition or that were recommended to me.

## Categories
---
- [Open Source Intelligence](/##Open-Source-Intelligence)
- [Cryptography](/##Cryptography)
- [Password Cracking](/##Password-Cracking)
- [Log Analysis](/##Log-Analysis)
- [Network Traffic Analysis](/##Network-Traffic-Analysis)
- [Forensics](/##Forensics)
- [Wireless Access Exploitation](/##Wireless-Access-Exploitation)
- [Scanning and Recon](/##Scanning-and-Recon)
- [Web Application Exploitation](/##Web-Application-Exploitation)
- [Enumeration and Exploitation](/##Enumeration-and-Exploitation)

## Appendix
---
- [Kali Linux](##/Kali-Linux)
- [Python Virtual Environment](##/Python-Virtual-Environment)
- [Vim](##/Vim)
- [Additional Resources](##/Additional-Resources)


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
### Command Line OSINT Tools
- `exiftool`
### OSINT Misc. Information and Resources
- [50 Common Ports You Should Know](https://www.geeksforgeeks.org/50-common-ports-you-should-know/#)
- [Service Name and Transport Protocol Port Number Registry](https://www.iana.org/assignments/service-names-port-numbers/service-names-port-numbers.xhtml) — IANA
- [Google Dork Cheatsheet](https://gist.github.com/sundowndev/283efaddbcf896ab405488330d1bbc06)
- [List of DNS Record Types](https://en.wikipedia.org/wiki/List_of_DNS_record_types)
- [Google Hacking Database](https://www.exploit-db.com/google-hacking-database)


## Cryptography
---
### Online Cipher and Translation Cryptography Tools
- [cryptii](https://cryptii.com/) — Modular conversion, encoding, and encryption online.
- [dcode](https://www.dcode.fr/cipher-identifier) — Cipher Identifier
- [CacheSleuth](https://www.cachesleuth.com/multidecoder/) — Mutli Decoder
- [Base64 Converter](https://www.base64decode.org/)
- [Hex to ASCII Converter](https://www.rapidtables.com/convert/number/hex-to-ascii.html)
- [Octal to Text Converter](https://www.browserling.com/tools/octal-to-text)
- [CodeBeautify](https://codebeautify.org/) — Code Formatter, Decode, Convert
  - [ZLib Decompress Online](https://codebeautify.org/zlib-decompress-online)
  - [Number System Converter](https://codebeautify.org/all-number-converter)
  - [JSON Beautifier, Viewer](https://codebeautify.org/jsonviewer), [JSON Validator](https://codebeautify.org/jsonvalidator), [JSON Cheat Sheet](https://codebeautify.org/json-cheat-sheet)
  - [HTML Viewer](https://codebeautify.org/htmlviewer)
  - [Image to Base64](https://codebeautify.org/image-to-base64-converter) / [Base64 to Image](https://codebeautify.org/base64-to-image-converter)
  - [HEX to Decimal](https://codebeautify.org/hex-decimal-converter) / [Decimal to Hex
  - [Binary to Text](https://codebeautify.org/binary-to-text), [Binary to Decimal](https://codebeautify.org/binary-decimal-converter)
  - [ASCII to Text](https://codebeautify.org/ascii-to-text)
  - [Encryption/Decryption](https://codebeautify.org/encrypt-decrypt)
  - ...and more
### Online Steganography Tools
- [StegOnline](https://stegonline.georgeom.net/upload) — Online Steg Decoder
- [FotoForensics](https://fotoforensics.com/analysis.php?id=b4727b6206fb898a6ae76ea14d8d6ae4fc623752.110213)
  - Supported formats: JPEG, PNG, WebP, HEIC, and AVIF.
  - The "Hidden Pixels" analysis option is particularly useful.
### Online RSA Decryption Tools
- [Integer Factorization Calculator](https://www.alpertron.com.ar/ECM.HTM)
### Command Line Cryptography Tools
- [RsaCtfTool](https://github.com/RsaCtfTool/RsaCtfTool) — Uncipher data from weak public keys and attempt to recover the corresponding private key.
- `exiftool`
- `openssl`
### Cryptography Software
- [DIIT](https://diit.sourceforge.net/) — Digital Invisible Ink Toolkit



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
### Hashcat
---
- With known format SKY-ABCD-####: `hashcat -m 0 -a 3 hashes.txt SKY-ABCD-?d?d?d?d`
  - `-m 0` for MD5 hashes.
  - `-a 3` for brute force and mask attack mode.
Hashcat example hashes and associated codes found [here](https://hashcat.net/wiki/doku.php?id=example_hashes).
### Password Cracking Software
- [Ophcrack](https://ophcrack.sourceforge.io/) — Windows password cracker based on rainbow tables.




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
- `wc` "Word Count" gets a line count (followed by a word count and a byte count) of a file or text stream.
  - `wc example.txt` prints the number of lines, words, bytes in example.txt.
  - `-l` flag to print number of lines only.
  - `-c` flag to print number of bytes only.
  - `-w` flag to print number of words only. A word is defined as a string of characters delimited by spaces, tabs, or newline characters.
- `awk` is a tool used to manipulate data. It can be used to extract specific columns from data.
  - `cat example.txt | awk '{print #2}'` prints the second column in example.txt.
- `tail` prints the last several lines of a file.
  - `tail example.txt` prints the last lines of example.txt.




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
### Forensics Software


## Wireless Access Exploitation
---
### Command Line Wireless Access Exploitation Tools
- [Aircrack-ng Suite](https://aircrack-ng.org/documentation.html)
  - aircrack
- `Airplay`
- `Wireshark`



## Scanning and Reconnaissance
---
### Command Line Scanning and Reconnaissance Tools
- `nmap`
- `nc`
- `amap`
- `dirbust/dirb`
- `dir`
- `telnet`
- [`smtp-user-enum`](https://pentestmonkey.net/tools/user-enumeration/smtp-user-enum) — Username guessing tool primarily for use against the default SMTP service.
  - [Linux username wordlist](https://github.com/rapid7/metasploit-framework/blob/master/data/wordlists/unix_users.txt)


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


## Vim
---



## Additional Resources
--- 





