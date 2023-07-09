# NCL Tools and Resources
The [National Cyber League (NCL)](https://nationalcyberleague.org/) is a bi-annual, virtual, puzzle-based, capture-the-flag style cybersecurity competition for high school and undergraduate students. 

*From the [NCL About Page](https://nationalcyberleague.org/about):* "NCL offers a fun way to learn and apply your skills in a safe environment - but it’s so much more than that, because with their NCL Scouting Reports you can present credible proof to employers of your hands-on expertise."
An article from the Applied Cybersecurity Division at NIST describes the [National Cyber League NICE Framework Success Story](https://www.nist.gov/itl/applied-cybersecurity/nice/nice-framework-resource-center/nice-framework-success-story-national).  

Information on upcoming NCL Competitions can be found [here](https://nationalcyberleague.org/competition).


This is an unofficial, non-exhaustive list of tools I've found useful during the competition or that were recommended to me.

## Categories
- [**Open Source Intelligence**](/osint-tools#Open-Source-Intelligence)
  - [OSINT Web Resources](/#OSINT-Web-Resources)
  - [Command Line OSINT Tools](/#Command-Line-OSINT-Tools)
  - [OSINT Misc. Information and Resources](/#OSINT-Misc.-Information-and-Resources)
- [**Cryptography**](/#Cryptography)
  - [Online Cipher Identification and Decryption Tools](/#Online-Cipher-Identification-and-Decryption-Tools)
  - [Online Steganography Tools](/#Online-Steganography-Tools)
  - [Online RSA Decryption Tools](/#Online-RSA-Decryption-Tools)
  - [Command Line Cryptography Tools](/#Command-Line-Cryptography-Tools)
  - [Cryptography Software](/#Cryptography-Software)
  - [Additional Resources](/#Additional-Resources)
- [**Password Cracking**](/#Password-Cracking)
  - [Online Password Cracking Tools](/#Online-Password-Cracking-Tools)
  - [Command Line Password Cracking Tools](/#Command-Line-Password-Cracking-Tools)
  - [Hashcat](/#Hashcat)
  - [Wordlists and Rule Lists](/#Wordlists-and-Rule-Lists)
  - [Password Cracking Information and Resources](/#Password-Cracking-Information-and-Resources)
- [**Log Analysis**](/#Log-Analysis)
  - [Command Line Log Analysis Tools](/#Command-Line-Log-Analysis-Tools)
  - [Creating Programs to do Log Analysis](/#Creating-Programs-to-do-Log-Analysis)
- [Network Traffic Analysis](/#Network-Traffic-Analysis)
  - [Command Line Network Traffic Analysis Tools](/#Command-Line-Network-Traffic-Analysis)
  - [Network Traffic Analysis Resources and Information](/#Network-Traffic-Analysis-Resources-and-Information)
- [**Forensics**](/#Forensics)
  - [General Forensics Tools](/#General-Forensics-Tools)
  - [Steganography Tools](/#Steganography-Tools)
  - [Unzip, Extract Files](/#Unzip,-Extract-Files)
  - [General Forensics Command Line Analysis Tools](/#General-Forensics-Command-Line-Analysis-Tools)
  - [Disk Imaging, Log](/#Disk-Imaging,-Log)
  - [Binwalk](/#Binwalk)
  - [Forensics Resources and Information](/#Forensics-Resources-and-Information)
- [**Wireless Access Exploitation**](/#Wireless-Access-Exploitation)
  - [Graphical Wireless Access Exploitation Tools](/#Graphical-Wireless-Access-Exploitation-Tools)
  - [Command Line Wireless Access Exploitation Tools](/#Command-Line-Wireless-Access-Exploitation-Tools)
  - [Misc. Wireless Access Exploitation Tools](/#Misc.-Wireless-Access-Exploitation-Tools)
- [**Scanning and Reconnaissance**](/#Scanning-and-Reconnaissance)
  - [Command Line Scanning and Reconnaissance Tools](/#Command-Line-Scanning-and-Reconnaissance-Tools)
  - [Graphical Scanning and Reconnaissance Tools](/#Graphical-Scanning-and-Reconnaissance-Tools)
  - [Nmap](/#Nmap)
- [**Web Application Exploitation**](/#Web-Application-Exploitation)
  - [Command Line Web Application Exploitation Tools](/#Command-Line-Web-Application-Exploitation-Tools)
- [**Enumeration and Exploitation**](/#Enumeration-and-Exploitation)
  - [General Enumeration and Exploitation Tools](/#General-Enumeration-and-Exploitation-Tools)
  - [Command Line Enumeration and Exploitation Tools](/#Command-Line-Enumeration-and-Exploitation-Tools)
  - [Enumeration and Exploitation Information and Resources](/#Enumeration-and-Exploitation-Information-and-Resources)
- [**Appendix**](/#Appendix)
  - [Unsorted Tools](/#Unsorted-Tools)
  - [Command Line Commands](/#Command-Line-Commands)
  - [Kali Linux](/#Kali-Linux)
  - [Windows Subsystem for Linux](/#Windows-Subsystem-for-Linux)
  - [Python Virtual Environment](/#Python-Virtual-Environment)
  - [Background Commands and Persistent Sessions](/#Background-Commands-and-Persistent-Sessions)
  - [Additional Resources](/#Additional-Resources)
  - [NCL Strategies](/#NCL-Strategies)



## Open Source Intelligence

### OSINT Web Resources
- [exif.regex.info](exif.regex.info) — Metadata viewer
- [Google Reverse Image Search](images.google.com) — Reverse image search
- [Github](github.com) — Code repository (lol)
- [Shodan](shodan.io) — Search engine for web services
- [Censys](https://censys.io/) — Online scanner for websites and certificates.
- [Greynoise](greynoise.io) — IP reputation search
- [Maxmind](maxmind.com) — GeoIP lookup
- [web.archive.org](web.archive.org) — The Internet archive
- [Latitude and Longitude converter](https://www.fcc.gov/media/radio/dms-decimal) — Degrees Minutes Seconds to/from Decimal Degrees
- [Cert Logik](https://certlogik.com/decoder/) — CSR decoder and certificate decoder
- [Geocode 3 Word System](https://what3words.com/royal.grass.prep) — Geocode system labeling every 3 meter square of the world with a unique 3-word combination.
- [Online Exiftool](https://exif.tools/) — online file metadata extraction

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

### Online Cipher Identification and Decryption Tools
- [dcode](https://www.dcode.fr/cipher-identifier) — Cipher identifier
  - [Caesar Cipher](https://www.dcode.fr/caesar-cipher)
  - [Morse Code Translator](https://morsedecoder.com/)
  - [Letter Number Code](https://www.dcode.fr/letter-number-cipher)
  - [Braille Alphabet](https://www.dcode.fr/braille-alphabet)
  - [Atbash Cipher](https://www.dcode.fr/atbash-cipher)
  - [Polybius Square Cipher](https://www.cachesleuth.com/polybiussquare.html)
  - [Five Needle Telegraph Code](https://www.cachesleuth.com/fiveneedletelegraph.html)
  - [ASCII Shift Cipher](https://www.dcode.fr/ascii-shift-cipher)
  - [rot8000 Cipher](https://rot8000.com/Index) — "rotate alphabet 0x8000 places", Caesar Shift for Unicode.
- [cryptii](https://cryptii.com/) — Modular conversion, encoding, and encryption online.
- [CacheSleuth](https://www.cachesleuth.com/multidecoder/) — Mutli decoder
- Number Bases Converters and Translators
  - [Base64 Converter](https://www.base64decode.org/)
  - [Hex to ASCII Converter](https://www.rapidtables.com/convert/number/hex-to-ascii.html)
  - [Octal to Text Converter](https://www.browserling.com/tools/octal-to-text)
- [CodeBeautify](https://codebeautify.org/) — Code formatter, decode, convert
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
- [Stegano](https://futureboy.us/stegano/) — Steghide online.
- [Online Exiftool](https://exif.tools/) — Online file metadata extraction
- [Sonic Visualizer](https://www.sonicvisualiser.org/) — Visualization, analysis, and annotation of music audio recordings.

### Online RSA Decryption Tools
- [Integer Factorization Calculator](https://www.alpertron.com.ar/ECM.HTM)
- [Prime Factorization Calculator](https://www.calculatorsoup.com/calculators/math/prime-factors.php)
- [RSA Calculator](https://www.cs.drexel.edu/~jpopyack/Courses/CSP/Fa17/notes/10.1_Cryptography/RSA_Express_EncryptDecrypt_v2.html)
- [dcode RSA Cipher Calculator](https://www.dcode.fr/rsa-cipher)
  
### Command Line Cryptography Tools
- [Ciphy](https://github.com/Ciphey/Ciphey) — Automatically determine cipher and output result.
- [RsaCtfTool](https://github.com/RsaCtfTool/RsaCtfTool) — Uncipher data from weak public keys and attempt to recover the corresponding private key.
-   [ExifTool](https://exiftool.org/) — Meta information reader/writer
  - [File types and meta information formats supported by ExifTool](https://github.com/exiftool/exiftool)
  - `exiftool <filename>`
- [OpenSSL](https://www.openssl.org/) — Command line program for using cryptography functions of OpenSSL's crypto library from the shell.
  - [`openssl` Program Docs](https://www.openssl.org/docs/manmaster/man1/openssl.html#SYNOPSIS)
  - [XORTool](https://github.com/hellman/xortool) — Python tool to analyze multi-byte xor cipher.
    
### Cryptography Software
- [DIIT](https://diit.sourceforge.net/) — Digital Invisible Ink Toolkit
- [Gimp](https://www.gimp.org/) — "GNU Image Manipulation Platform"
  
### Additional Resources
- [Chart to Identify Number Bases](https://cryptokait.com/2020/05/27/summer-camp-2020-numerical-cryptography/)
- [Code Tables Index](https://www.cachesleuth.com/codes/) — Identify what character set is in a cipher.




## Password Cracking

### Online Password Cracking Tools
- [MD5 Hash Generator](https://www.md5hashgenerator.com/)
- [SHA256 Hash Generator](https://emn178.github.io/online-tools/sha256.html)
- [CrackStation](https://crackstation.net/) — Online password hash cracking
- [Hashes](https://hashes.com/en/decrypt/hash) — Decrypt MD5, SHA1, MySQL, NTLM, SHA256, MD5 Email, SHA256 Email, SHA512 hashes.
  
### Command Line Password Cracking Tools
- [`hash-identifier`](https://www.kali.org/tools/hash-identifier/)
- `hashcat` (more below)
- [`fcrackzip`](https://www.kali.org/tools/fcrackzip/) — Zip password cracker
- [John the Ripper](https://www.openwall.com/john/) — Password cracker
- [Ophcrack](https://ophcrack.sourceforge.io/) — Windows password cracker based on rainbow tables.
  
### Hashcat
- Flag options (control character sets for brute force attacks)
  - `?l` — Charset: abcdefghijklmnopqrstuvwxyz
  - `?u` — Charset: ABCDEFGHIJKLMNOPQRSTUVWXYZ
  - `?f` — Charset: 0123456789
  - `?h` — Charset: 0123456789abcdef
  - `?H` — Charset: 0123456789ABCDEF
  - `?s` — Charset: !”#$%&'()*+,-./:;<=>?@[\]^_`{|}~
  - `?a` — Charset: ?l?u?d?s
  - `?b` — Charset: 0x00 – 0xff
- Attack modes
  - `-a 0` — Dictionary attack (tries all lines contained in a given file as passwords)
  - `-a 1` — Combinator attack (tries combinations of words from wordlist)
  - `-a 3` — Brute-Force attack 
  - `-a 6` — Hybrid Wordlist + Mask
  - `-a 7` — Hybrid Mask + Wordlist
  - `-a 9` — Association 
- With known format SKY-ABCD-####:
  ```bash
  hashcat -m 0 -a 3 hashes.txt SKY-ABCD-?d?d?d?d
  ```
  - `-m 0` for MD5 hashes.
  - `-a 3` for brute force and mask attack mode.
- Using the rockyou wordlist:
  ```bash
  hashcat -m 0 -a 0 hashes.txt rockyou.txt
  ```
- [Hybrid attacks](https://hashcat.net/wiki/doku.php?id=hybrid_attack)
- [Rule-based attacks](https://hashcat.net/wiki/doku.php?id=rule_based_attack)
- [Extracting WPA and WPA2 hashes from PCAPs for use with hashcat](https://hashcat.net/wiki/doku.php?id=hccapx)
- Hashcat example hashes and associated codes found [here](https://hashcat.net/wiki/doku.php?id=example_hashes).

### Wordlists and Rule Lists
- [Wordlists in hashcat](https://www.kali.org/tools/wordlists/)
  - To see what wordlists are available: `wordlists -h`
- [SecLists](https://github.com/danielmiessler/SecLists/tree/master/Passwords) — GitHub Repo full of wordlists.
- [Wordlists, Password Lists, Dictionaries](https://wiki.skullsecurity.org/index.php/Passwords)
- [cewl](https://www.kali.org/tools/cewl/) — Useful for generating wordlists.
- Combine wordlists with hashcat:
  ```bash
  /usr/share/hashcat-utils/combinator.bin firstwordlist.txt secondwordlist.txt > combined_wordlist.txt
  ```
- Rule lists in hashcat: `ls /usr/share/hashcat/rules`
  - Most powerful: `dive.rule`

### Password Cracking Information and Resources
- [CryptoKait article: Taking Password Cracking to the Next Level](https://cryptokait.com/2020/09/02/taking-password-cracking-to-the-next-level/)
- [How to Perform a Rule Based Attack on Hashcat](https://www.4armed.com/blog/hashcat-rule-based-attack/)

It may be helpful to run some of these commands in the background or use a persistent session. 
Information about these options is found [in the Appendix](/#Background-Commands-and-Persistent-Sessions)


## Log Analysis

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
  - grep IP address:
    ```bash
    grep -E '[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}' example.txt
    ```
  - grep only valid IP address:
    ```bash
    grep -E '^((25[0-5]|2[0-4][0-9]|[1]?[1-9][0-9]?).){3}(25[0-5]|2[0-4][0-9]|[1]?[1-9]?[0-9])$' example.txt
    ```
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

### SQLite
- [SQLite Browser](https://sqlitebrowser.org/dl/)
- [`sqlite3 <file.sqlite>`](https://www.sqlite.org/cli.html)
  - `.tables` to see a list of tables.
  - `.index` to see index.
  - `.schema` to see a list of schema.
  - `.databases`
    
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

### Command Line Network Traffic Analysis Tools
- `TCPDump` —
- `Wireshark` — 
- `Aircrack` — 

### Network Traffic Analysis Resources and Information
- [How to display WEP key from PCAP file in Wireshark? (Stack Overflow)](https://stackoverflow.com/questions/55667434/how-to-display-wep-key-from-pcap-file-in-wireshark)
- [How to convert rtpdump video file to mp4? (Stack Overflow)](https://stackoverflow.com/questions/42564983/how-to-convert-rtpdump-video-file-to-mp4)





## Forensics

### General Forensics Tools
- [HexEd.it](https://hexed.it/) — Online hex editor
- [Autopsy Forensic Browser](https://www.kali.org/tools/autopsy/) — Digital forensics platform
  - [Autopsy Tutorial (blog post)](https://cryptokait.com/2021/03/08/digging-into-autopsy-forensics/)
- [pspy](https://github.com/DominicBreuker/pspy) — Low privilege process snooper.
- [Audacity](http://sourceforge.net/projects/audacity/) — Analyze sound files.
  
### Steganography
- [FotoForensics](https://fotoforensics.com/analysis.php?id=b4727b6206fb898a6ae76ea14d8d6ae4fc623752.110213)
  - Supported formats: JPEG, PNG, WebP, HEIC, and AVIF.
  - The "Hidden Pixels" analysis option is particularly useful.
- [Binwalk](/#Binwalk) — Search a binary image for embedded files, executable code.
- [Foremost](https://tools.kali.org/forensics/foremost) — May catch something Binwalk misses.
- [steghide](https://github.com/StefanoDeVuono/steghide) — Hides and extracts data from files.
- [zsteg](zsteg ) — Find steganography in PNG and BMP files. 
  - `zsteg -a` runs every detection method on the given file.
  - `zsteg -E` extracts data with the given payload.
- [stegsolve](https://github.com/zardus/ctf-tools/tree/master/stegsolve) — Can be used to find hidden information in files.
- `fft` (Fast Fourier Transform)
- [stegoveritas](https://github.com/bannsec/stegoVeritas) — Carve and extract; similar to zsteg.
- [stegdetect](https://linux.die.net/man/1/stegdetect) — Statistically determine if steganograhpic content is present and how.
- [Snow](https://sbmlabs.com/notes/snow_whitespace_steganography_tool) — Whitespace steganography tool
- [StegCracker](https://github.com/Paradoxis/StegCracker) — Brute-force utility to uncover hidden data inside files.

### Unzip, Extract Files
- [7-Zip](https://www.7-zip.org/) — File archiver with a high compression ratio (and opens just about anything)
- `unzip filename.docx -d out` to unzip .docx files to see what's inside.
- `gzip -d file.gz` (or `gzip -dk file.gz` to keep compressed file) — Unzip `gz` File
- `gunzip file.gz` — Unzip `gz` file (this command is essentially an alias to `gzip -d`.
- `tar -xf archive.tar.gz` to extract a `tar.gz` file.
- `unrar` —
  
### General Forensics Command Line Analysis Tools
- `file` — Determine the type of a file.
  - `file -i` — View mime type of file.
  - `file -z` — Try to look inside compressed files.
- [Exif Tool](http://www.sno.phy.queensu.ca/~phil/exiftool/) — Read, write, edit file metadata.
- [Exif](http://manpages.ubuntu.com/manpages/trusty/man1/exif.1.html) — Shows EXIF information in JPEG files.
- `xxd` — Dump file in hex format.
- [Binwalk](/#Binwalk) — Search a binary image for embedded files, executable code.
- [Foremost](https://tools.kali.org/forensics/foremost) — May catch something Binwalk misses.
- [Pngcheck](http://www.libpng.org/pub/png/apps/pngcheck.html) — Verifies PNG integrity, dump chunk-level info in human-readable form. 
- [scalpel](https://www.kali.org/tools/scalpel/#scalpel) — fast file carver that reads database of header and footer definitions and extracts matching files from a set of image files or raw device files.
- [identify](https://imagemagick.org/script/identify.php) — Image format and characteristics
  - Supported file formats include JPEG, PNG, GIF, TIFF, PDF.
- [Extundelete](http://extundelete.sourceforge.net/) — Recover lost data from mountable images.
- [PDF Streams Inflater](http://malzilla.sourceforge.net/downloads.html) — Find, extract zlib files compressed in PDF files.
- [pdfimages](https://www.xpdfreader.com/pdfimages-man.html) — PDF Image Extractor
  - `pdfimages` saves images from PDF as PPM, PGM, PBM, or JPEG files.
  - `pdfimages -f <number>` specifies the first page to scan.
  - `pdfimages -l <number>` specifies the last page to scan.
  - `pdfimages -j` — Images in DCT format saved as JPEG files; non-DCT images saved in PBM/PGM/PPM format as usual.

### Disk Imaging, Log
- [FTK Imager](https://www.exterro.com/ftk-product-downloads/ftk-imager-version-4-7-1) — Saves image of hard disk in a file or segments. Calculates MD5 and SHA1 hash values. 
- [LogFileParser](https://github.com/jschicht/LogFileParser) — Parser for LogFile on NTFS.
- [NTFS Log Tracker](https://sites.google.com/site/forensicnote/ntfs-log-tracker) — parse $LogFile, $UsnJrnl:$J of NTFS and carve UsnJrnl record in multiple files(unallocated dump, file slack, pagefile.sys, memory dump, vss, ...).
  - [Info about using NTFS Log Tracker](http://forensicinsight.org/wp-content/uploads/2013/06/F-INSIGHT-NTFS-Log-TrackerEnglish.pdf)

### Binwalk
[Binwalk](https://github.com/ReFirmLabs/binwalk) — Search a binary image for embedded files, executable code.
- Scan a binary file:
  ```bash
  binwalk <filename>
  ```
- Extract files from a binary, specifying the output directory:
  ```bash
  binwalk --extract --directory <output_directory> <filename>
  ```
- Recursively extract files from a binary limiting the recursion depth to 2:
  ```bash
  binwalk --extract --matryoshka --depth [2] <filename>
  ```
- Extract files from a binary with the specified file signature:
  ```bash
  binwalk -dd '[png image:png]' <filename>
  ```
- Analyze the entropy of a binary, saving the plot with the same name as the binary and .png extension appended:
  ```bash
  binwalk --entropy --save <filename>
  ```
- Combine entropy, signature, and opcodes analysis in a single command:
  ```bash
  binwalk --entropy --signature --opcodes <filename>
  ```

### Forensics Resources and Information
- [Decoding Identifying Printer Information](https://www.eff.org/files/filenode/printers/ccc.pdf)
- [Find Hidden Hyperlinks in Word Document](https://www.techwalla.com/articles/how-to-find-hyperlinks-in-a-word-document)


## Wireless Access Exploitation

### Command Line Wireless Access Exploitation Tools
- [Aircrack-ng Suite](https://aircrack-ng.org/documentation.html)
  - `aircrack-ng`
- `Airplay`
- [`tshark [options] ...`](https://www.wireshark.org/docs/man-pages/tshark.html) to dump and analyze network traffic.
- `capinfos [options] <infile> ...` to print information about capture files.
- `captype [options] <infile> ...` to print types of capture files.
- `dumpcap [options] ...` to dump network traffic. 
- `mmdbresolve -f db_file [-f db_file ...]` to read IPv4 and IPv6 addresses and print their IP geolocation information.
- `text2pcap [options] <infile> <outfile>` to generate a capture file from an ASCII hexdump of packets.

### Graphical Wireless Access Exploitation Tools
- [Wireshark](https://www.wireshark.org/)
  - `wireshark [options] ... [ <infile> ]` to interactively dump and analyze network traffic.

### Misc. Wireless Access Exploitation Resources
- [CryptoKait article: Secret Information in Network Traffic Logs: NTA for NCL](https://cryptokait.com/2020/02/19/secret-information-in-network-traffic-logs-nta-for-ncl/)
- Packet Dissection: [write your own dissector](https://www.wireshark.org/docs/wsdg_html_chunked/ChDissectAdd.html)




## Scanning and Reconnaissance

### Command Line Scanning and Reconnaissance Tools
- [Nmap](/#Nmap)
- `nc` —
- `amap` — 
- `dirbust/dirb/dir` —
- [Dirbuster](https://www.kali.org/tools/dirbuster/) —
- `telnet` —
- [`smtp-user-enum`](https://pentestmonkey.net/tools/user-enumeration/smtp-user-enum) — Username guessing tool primarily for use against the default SMTP service.
  - [Linux username wordlist](https://github.com/rapid7/metasploit-framework/blob/master/data/wordlists/unix_users.txt)

### Graphical Scanning and Reconnaissance Tools
- [Zenmap](https://nmap.org/zenmap/) — A graphical user interface for Nmap.

### Nmap
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
  ```
- Range of ports:
  ```bash
  nmap -p 76-973 192.164.0.1
  ```
- Top Ports:
  ```bash
  nmap --top-ports 10 scanme.nmap.org
  ```
- Scanning from a file with a list of IP addresses:
  ```bash
  nmap -iL /input_ips.txt
  ```



## Web Application Exploitation

### Command Line Web Application Exploitation Tools
- `wget`
- `curl`
- [SQLMap](https://github.com/sqlmapproject/sqlmap) — Automatic SQL injection tool
- [w3af](https://docs.w3af.org/en/latest/) — Web Application Attack and Audit Framework
- `wpscan` —
- `burpsuite` —
- `hackbar` —
- `editthiscookie` —
- `firebug` —




## Enumeration and Exploitation

### General Enumeration and Exploitation Tools
- [Ghidra](https://ghidra-sre.org/) — Software reverse engineering suite of tools.
- [GNU Project Debugger (GDB)](https://www.sourceware.org/gdb/) — See what a program does as it executes, or what it was doing when it crashed.
- [pwndbg](https://github.com/pwndbg/pwndbg) — Python module loaded directly into GDB; provides suite of utilitie, crutches to hack around GDB.

### Command Line Enumeration and Exploitation Tools
- `uncompyle6` —
- `strings` —

### Enumeration and Exploitation Information and Resources
- [List of Unicode Characters](https://en.wikipedia.org/wiki/List_of_Unicode_characters)
- [LD_PRELOAD trick](http://www.goldsborough.me/c/low-level/kernel/2016/08/29/16-48-53-the_-ld_preload-_trick/)




## Appendix

### Unsorted Tools

- [pwntools](https://docs.pwntools.com/en/stable/) — Python library for interacting with ctf challenges, focus on pwning.
- [ffmpeg](https://ffmpeg.org/) — Record, convert, stream audio and video.



### Command Line Commands

- `>` takes the standard output of the command on the left and redirects it to the file on the right.
- `>>` takes the standard output of the command on the left and *appends* it to the file on the right.
- `<` takes the standard input from the file on the right and inputs it into the program on the left.
- `|` is a "pipe". It takes the standard output of the command on the left, and *pipes* it as standard input to the command on the right.
- `alias` allows you to create keyboard shortcuts (aliases).
- `grep` stands for "global regular expression print". It searches files for lines that match a pattern and returns the results. Case sensitive.
  - `grep -i` for case insensitive grep.
  - `grep -R` ("Recursive") searches all files in a directory and outputs filenames and lines containing matched results. 
  - `grep -Rl` ("Recursive" and "files with matches") searches all files in a directory and outputs only filenames with matched results.
- `ls` lists all files and directories in the working directory.
  - `ls -a` lists all contents in working directory, includes hidden files and directories.
  - `ls -l` lists all contents of a directory in long format.
  - `ls -t` orders files and directories by the time they were last modified.
- `pwd` "print working directory"
- `rm` deletes files.
  - `rm -r` deletes a directory and all its child directories. 
- `sed` "stream editor". Accepts standard input and modifies it based on an *expression* before displaying it as output data.
- `sort` takes a file name or standard input and orders each line alphabetically, printing it to standard output.
- `source` activates changes in bash profile for current session.
- `touch` creates a new empty file in the working directory. 
- `uniq` "unique". Takes a filename or standard input and prints out every line, removing any exact duplicates.



### Kali Linux 
- [Kali Tools Documentation](https://www.kali.org/tools/)



### Windows Subsystem for Linux

For information about using Kali via. WSL for the NCL competition, check out [this article from CryptoKait](https://cryptokait.com/2020/08/19/ncl-and-wsl-leaving-the-kali-vm-behind/).
If you want to install WSL, instructions can be found [here](https://learn.microsoft.com/en-us/windows/wsl/install). 
The Kali Linux installation on WSL is a [minimum install setup](https://www.kali.org/docs/troubleshooting/common-minimum-setup/). 
That means you'll probably want to [install Kali Linux Metapackages](https://www.kali.org/docs/general-use/metapackages/).




### Python Virtual Environment
 
Python documentation on how to create a virtual environment with `venv` can be found [here](https://docs.python.org/3/library/venv.html).
Information on installing packages with `pip` in a virtual environment can be found [here](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/).



### Background Commands and Persistent Sessions

To run a command in the background, add ampersand to the end of the command:
```bash
command &
```
To suppress the `stdout` and `stderr` messages, use:
```bash
command > /dev/null 2>&1 &
```
To display the status of all stoped and background jobs in the current shell session:
```bash
jobs -l
```
To bring a background process to the foreground, use the `fg` command (or `fg %1` if you have multiple background jobs.

To terminate the background process, use the `kill` command followed by the process ID (which can be obtained through the `jobs -l` command, above. In this example it's 12928):
```bash
kill -9 12928
```

Generally, if connection drops or you exit the shell session, the background process terminates. 
To keep the process running, use the `disown` command or start the process with the `nohup` command.

Alternatively, use [Tmux](https://linuxize.com/post/getting-started-with-tmux/) ("terminal multiplexer") to switch between multiple programs in one terminal. 
Tmux sessions are persistent; programs will continue to run even if you exit the shell or are disconnected.




### Additional Resources
A bank of CTF resources and tools can be found [here](https://github.com/zardus/ctf-tools).




### NCL Strategies

CryptoKait's article on [Top 10 Dos and Don'ts for the National Cyber League Games](https://cryptokait.com/2019/10/15/top-10-dos-and-donts-for-the-national-cyber-league-games/) from 2019 has tips from NCL Player Ambassadors, Cyber Skyline Game-makers, etc. on how to be successful during the games.

