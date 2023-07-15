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
  - `?s` — Charset: `!”#$%&'()*+,-./:;<=>?@[\]^_{|}~`
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


## PDF Files
- `pdfcrack --wordlist=rockyou.txt filename.pdf`
- `pdf-parser`
- `pdf2john`
- `john`
- [Writeup of Cracking Encrypted PDFs](https://blog.didierstevens.com/2017/12/26/cracking-encrypted-pdfs-part-1/)
