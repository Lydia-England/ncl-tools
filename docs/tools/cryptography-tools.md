# Cryptography

---

## Number Bases Converters and Translators
- [Base64 Converter](https://www.base64decode.org/)
- [Hex to ASCII Converter](https://www.rapidtables.com/convert/number/hex-to-ascii.html)
- [Octal to Text Converter](https://www.browserling.com/tools/octal-to-text)

---

# Cipher Identification and Decryption Tools

## dCode
dCode.fr is a collection of hundreds of tools to help solve ciphers, codes, puzzles, etc. 
Check out the [online dCode Cipher Identifier](https://www.dcode.fr/cipher-identifier) if you're not sure how a message is encrypted. 
Or check out the [list of all available dCode tools](https://www.dcode.fr/tools-list).

### Commonly used dCode cipher tools: 
- [Caesar Cipher](https://www.dcode.fr/caesar-cipher)
  - Substitution cipher: letters in the alphabet are shifted by some fixed number of spaces to yield an encoding alphabet. 
- [Morse Code Translator](https://morsedecoder.com/)
  - Encodes text characters as sequences of two different signal durations, called dots and dashes (or dits and dahs). 
  - Example: `.... . .-.. .-.. ---` is "Hello" in Morse code.
- [Letter Number Code](https://www.dcode.fr/letter-number-cipher)
  - Replaces each letter with its position in the alphabet. 
  - "Space" character is often encoded as a zero, but may be encoded as something else (or not encoded at all).
  - Example: "Hello World" is encrypted as: `8-5-12-12-15-0-23-15-18-12-4`
- [Braille Alphabet](https://www.dcode.fr/braille-alphabet)
  - Braille is a tactile writing system used by people who are visually impaired.
  - Each letter corresponds to a specific pattern of raised dots.
- [Atbash Cipher](https://www.dcode.fr/atbash-cipher)
  - The Atbash cipher encodes a message with the reverse of the alphabet. 
  - Example: "Hello World" is encrypted as: `Svool Dliow`
- [Polybius Square Cipher](https://www.cachesleuth.com/polybiussquare.html)
  - The Polybius square places all letters in a grid; each letter is represented by its coordinates in the grid. 
  - A *key* could be used to reorder the alphabet in the square, with the letters (without duplicates) being placed at the beginning and the remaining letters following it in alphabetical order.
- [Five Needle Telegraph Code](https://www.cachesleuth.com/fiveneedletelegraph.html)
  - The Five Needle Telegraph Code (a.k.a. the Cooke and Wheatstone Telegraph) is represented by three characters `\|/` in a set of 5. 
  - Example: "Hello" is encrypted as: `/\||| /|\|| |||/\ |||/\ ||\/|`
- [ASCII Shift Cipher](https://www.dcode.fr/ascii-shift-cipher)
  - The ASCII shift cipher is like the Caesar cipher, but the ASCII table is used instead of the Latin alphabet, yielding 127 different offsets.
  - Example: "Hello World" is encrypted as: `08 25 2C 2C 2F 60 17 2F 32 2C 24` (with a shift of 64, output in hexadecimal).
- [rot8000 Cipher](https://rot8000.com/Index) 
  - "rotate alphabet 0x8000 places". 
  - Variant of ROT-13 or ROT-47 adapted to Unicode with a rotation of 0x8000 (hexadecimal value).
  - Example: "Hello World" is encrypted as: `籛籘籝籁簹簹簹`.


## Code Beautify
[CodeBeautify](https://codebeautify.org/) is an online Code formatter, decoder, converter.
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


## Misc. Command Line Cryptography Tools
- [Ciphy](https://github.com/Ciphey/Ciphey) 
  - Automatically determine cipher and output result.
- [FeatherDuster](https://github.com/nccgroup/featherduster)
  - Tool for breaking crypto (identifying and exploiting weak cryptosystems).
  - Run with: `featherduster [ciphertext file 1] ... [ciphertext file n]`
- [Cryptanalib](https://github.com/nccgroup/featherduster)
  - Part of the Featherduster project; can be used independently of FeatherDuster.
  - Used to make Python-based crypto attack tools.
  - Documentation accessed through the Python `help()` function.
- [Cryptanalib3](https://pypi.org/project/cryptanalib3/)
  - Python3 fork of `cryptanalib` module from FeatherDuster project. 
  - Standalone module for performing cryptanalysis and cryptographic exploit development.
  - Import: Launch Python3 and `import ca3`.
  - Cryptanalib3 attempts to decode, identify, and look for indicators of vulnerability with th `analyze_ciphertext()` function.


## Misc. Other decoders, etc.
- [CacheSleuth](https://www.cachesleuth.com/multidecoder/) 
  - Mutli decoder
- [CyberChef](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwijlaDt3oyAAxWxGjQIHXlgA28QFnoECA4QAQ&url=https%3A%2F%2Fgchq.github.io%2FCyberChef%2F&usg=AOvVaw3cJhXGWs_4gKkmjmhQLSNC&opi=89978449) 
  - Web app for encryption, encoding, compression, and data analysis. 
  - Build "recipes" to analyze data.
  - `Magic` option tries to identify the cipher; attempts many decoding methods.
- [cryptii](https://cryptii.com/) 
  - Modular conversion, encoding, and encryption online
- [Shamir's Secret Sharing](http://christian.gen.co/secrets/)
  - SSS is a secret sharing algorithm for distributing a secret among a group. 
  - The secret cannot be revealed unless a quorum of the group acts together to pool their knowledge.
- [Boxentriq](https://www.boxentriq.com/)
  - Online code-breaking, cipher, and logic puzzles solving tools.
  - Classic ciphers, text and word tools, analysis tools, modern ciphers, steganography, encodings, math, alphabets, etc.
- [List of Online Tools for Ciphers and Codes](https://rumkin.com/tools/cipher/)
- [Identify Encryption or Number Base](https://book.hacktricks.xyz/crypto-and-stego/crypto-ctfs-tricks)


## Brute force OpenSSL encrypted file
- [Bruteforce Salted OpensSL](https://github.com/glv2/bruteforce-salted-openssl)
  - Try to find the password of a file that was encrypted with the `openssl` command.
    - OpenSSL encryption example: `openssl enc -aes256 -salt -in clear.file -out encrypted.file`
  - Can be used either to try all the passwords in a file or to try all possible passwords in a given charset.
- [Easy Brute Force OpenSSL CTF](https://github.com/carlospolop/easy_BFopensslCTF)
  - Bash script that given a password (or wordlist) tries to decrypt an OpenSSL encrypted file using several algorithms.


---

# Steganography Tools
For steganography tools, visit the [Steganography Tools Page](/steg-tools.md)

---

# RSA Decryption Tools
- [Integer Factorization Calculator](https://www.alpertron.com.ar/ECM.HTM)
- [Prime Factorization Calculator](https://www.calculatorsoup.com/calculators/math/prime-factors.php)
- [RSA Calculator](https://www.cs.drexel.edu/~jpopyack/Courses/CSP/Fa17/notes/10.1_Cryptography/RSA_Express_EncryptDecrypt_v2.html)
- [dcode RSA Cipher Calculator](https://www.dcode.fr/rsa-cipher)
- [Carmichael Function Calculator](https://comnuan.com/cmnn02/cmnn02006/cmnn02006.php)
- [RsaCtfTool](https://github.com/RsaCtfTool/RsaCtfTool) 
  - Uncipher data from weak public keys and attempt to recover the corresponding private key.
  

