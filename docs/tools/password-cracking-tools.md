# Password Cracking

## Online Password Cracking Tools
- [MD5 Hash Generator](https://www.md5hashgenerator.com/)
- [SHA256 Hash Generator](https://emn178.github.io/online-tools/sha256.html)
- [CrackStation](https://crackstation.net/) 
  - Online password hash cracking
- [Hashes](https://hashes.com/en/decrypt/hash) 
  - Decrypt MD5, SHA1, MySQL, NTLM, SHA256, MD5 Email, SHA256 Email, SHA512 hashes.
  - Note that the output may not be listed in the same order the input was listed in.
- [MD5 Decrypt](https://md5decrypt.net/en/)
  - Basic decryption of MD5, SHA1, SHA256, SHA384, SHA512, NTLM, COR, BCrypt, Blowfish, and Whirlpool hashes.
- [ranbowtables.it64.com](http://rainbowtables.it64.com/)
  - Rainbow table attack on Microsoft Windows LM hashes. 
  

## Command Line Password Cracking Tools
- [Hash Identifier](https://www.kali.org/tools/hash-identifier/)
  - Software to identify different types of hashes used to encrypt data and especially passwords. 
  - Usage: enter `hash-identifier` in the command line. Enter hashes when prompted.
- [HashID](https://www.kali.org/tools/hashid/)
  - Identify different types of hashes used to encrypt data and especially passwords.
  - Usage: enter `hashid <hash>` in the command line, where `<hash>` can be a single hash or a file containing hashes.
- [Hashcat](https://hashcat.net/wiki/)
  - More information below.
- [fcrackzip](https://www.kali.org/tools/fcrackzip/) — Zip password cracker
  - To use fcrackzip and the rockyou wordlist to crack the password on a ZIP file, enter: 
  ```bash
  fcrackzip -v -u -D -p rockyou.txt archive.zip
  ```
    - `-u` (`-use-unzip`) helps with false positives
    - `-D` (`-dictionary`) selects dictionary mode
    - `-p` (`-init-password string`) use to select the rockyou.txt file
    - `-v` (`-verbose`) not required
- [John the Ripper](https://www.openwall.com/john/) — Password cracker
- [Ophcrack](https://ophcrack.sourceforge.io/) — Windows password cracker based on rainbow tables.
  

## Hashcat
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


## Wordlists and Rule Lists


## PDF Files
- `pdfcrack --wordlist=rockyou.txt filename.pdf`
- `pdf-parser`
- `pdf2john`
- `john`
- [Writeup of Cracking Encrypted PDFs](https://blog.didierstevens.com/2017/12/26/cracking-encrypted-pdfs-part-1/)


## Windows Hashes 
  - LM, NTLM, Net-NTLMv2
  - Output from `hash-identifier` may look like: `SAM - (LM_hash:NT_hash)`
  - [Article on cracking Windows hashes](https://medium.com/@petergombos/lm-ntlm-net-ntlmv2-oh-my-a9b235c58ed4)


