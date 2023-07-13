# Cryptography

## Number Bases Converters and Translators
---
- [Base64 Converter](https://www.base64decode.org/)
- [Hex to ASCII Converter](https://www.rapidtables.com/convert/number/hex-to-ascii.html)
- [Octal to Text Converter](https://www.browserling.com/tools/octal-to-text)




# Cipher Identification and Decryption Tools
---

## dCode
dCode.fr is a collection of hundreds of tools to help solve ciphers, codes, puzzles, etc. 
Check out the [online dCode Cipher Identifier](https://www.dcode.fr/cipher-identifier) if you're not sure how a message is encrypted. 
Or check out the [list of all available dCode tools](https://www.dcode.fr/tools-list).

Commonly used dCode cipher tools: 
- [Caesar Cipher](https://www.dcode.fr/caesar-cipher)
- [Morse Code Translator](https://morsedecoder.com/)
- [Letter Number Code](https://www.dcode.fr/letter-number-cipher)
- [Braille Alphabet](https://www.dcode.fr/braille-alphabet)
- [Atbash Cipher](https://www.dcode.fr/atbash-cipher)
- [Polybius Square Cipher](https://www.cachesleuth.com/polybiussquare.html)
- [Five Needle Telegraph Code](https://www.cachesleuth.com/fiveneedletelegraph.html)
- [ASCII Shift Cipher](https://www.dcode.fr/ascii-shift-cipher)
- [rot8000 Cipher](https://rot8000.com/Index) — "rotate alphabet 0x8000 places", Caesar Shift for Unicode.




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


## Misc. Other decoders, etc.
- [CacheSleuth](https://www.cachesleuth.com/multidecoder/) — Mutli decoder
- [CyberChef](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwijlaDt3oyAAxWxGjQIHXlgA28QFnoECA4QAQ&url=https%3A%2F%2Fgchq.github.io%2FCyberChef%2F&usg=AOvVaw3cJhXGWs_4gKkmjmhQLSNC&opi=89978449) — Web app for encryption, encoding, compression, and data analysis. Build "recipes" to analyze data.
- [cryptii](https://cryptii.com/) — Modular conversion, encoding, and encryption online

- [List of Online Tools for Ciphers and Codes](https://rumkin.com/tools/cipher/)





# Steganography Tools
---

*Note: Many important Forensics tools also apply to cryptography (especially steganography) challenges. If you're stuck, check the Forensics Tools page.*

## Online Stego Tools
- [StegOnline](https://stegonline.georgeom.net/upload) — Online Steg Decoder
- [FotoForensics](https://fotoforensics.com/analysis.php?id=b4727b6206fb898a6ae76ea14d8d6ae4fc623752.110213)
  - Supported formats: **JPEG**, **PNG**, **WebP**, **HEIC**, and **AVIF**.
  - The "Hidden Pixels" analysis option is particularly useful.
- [Stegano](https://futureboy.us/stegano/) — Steghide online
- [Online Exiftool](https://exif.tools/) — Online file metadata extraction
- [inlite](https://online-barcode-reader.inliteresearch.com/) — QR Code, Barcode, Data Matrix, Driver License reader
- [Image to Binary Converter (dcode)](https://www.dcode.fr/binary-image) — Useful for QR codes
- [Image Error Level Analyser](https://29a.ch/sandbox/2012/imageerrorlevelanalysis/) — Identify manipulations to compressed (JPEG) images by detecting distribution of error introduced after resaving the image at a specific compression rate.
- [Magic Eye Solver/Viewer](http://magiceye.ecksdee.co.uk/) — View hidden image; includes slider to move towards/away from the magic eye.
- [Twitter Secret Messages](https://holloway.nz/steg/) — Hide/extract secret messages in tweets (or any text) with *steg-of-the-dump.js*.
- [Hidden data in spaces](https://www.irongeek.com/i.php?page=security/unicode-steganography-homoglyph-encoder)


## Command Line Stego Tools
- [Identify](https://linux.die.net/man/1/identify) — 
  - 
- [Steghide](https://www.kali.org/tools/steghide/) — 
  - **JPEG**, **BMP**, **WAV**, **AU**
- [Zsteg](https://github.com/zed-0xff/zsteg) — Detect stegano-hidden data in PNG and BMP
  - **PNG**, **BMP**
- [stegoVeritas]() — 
  - **JPG**, **PNG**, **GIF**, **TIFF**, **BMP**
- [Stegpy](https://github.com/dhsdshdhk/stegpy) — Encoding information in information in image, audio files
  - **PNG**, **BMP**, **GIF**, **WebP**, **WAV**
- [Pngcheck](http://www.libpng.org/pub/png/apps/pngcheck.html) — Get details on a PNG file (or find out if it's actually something else)
  - **PNG**


## Fast Fouier Transform (FFT) Steganography Tools
- [Imaging Web Demo - FFT Tool](http://bigwww.epfl.ch/demo/ip/demos/FFT/) — Online FFT Tool
- [Ejectamenta](https://www.ejectamenta.com/Fourifier-fullscreen/) — Online FFT Tool
- [FFTStegPic](https://github.com/0xcomposure/FFTStegPic) — Python script for digital image stego with FFT


## Audio and Video Stego Tools
- [Sonic Visualizer](https://www.sonicvisualiser.org/) — Visualization, analysis, and annotation of music audio recordings.
  - If you're stuck, always check the spectrogram of the audio.
- [Sonic Lineup](https://www.sonicvisualiser.org/sonic-lineup/index.html) — Rapid visualisation of multiple audio files containing versions of the same source material. Part of the Sonic Visualizer family of applications.
- [Sonic Annotator](https://vamp-plugins.org/sonic-annotator/) — Batch tool for feature extraction and annotation of audio files using [Vamp plugins](https://vamp-plugins.org/index.html). Part of the Sonic Visualizer family of applications.
- [Detect DTMF Tones (file upload)](http://dialabc.com/sound/detect/index.html) — 
- [Detect DTMF Tones (demo)](https://unframework.github.io/dtmf-detect/) — 
- [Wavsteg](https://github.com/ragibson/Steganography#WavSteg) — 
  - Supported formats: **WAV**
  - Useful command:
  Extracts to an ouput file (taking only 1 lsb)
  ```bash
  python3 WavSteg.py -r -b 1 -s soundfile -o outputfile
  ```
  - Useful command:
  Extracts to an ouput file (taking only 2 lsb)
  ```bash
  python3 WavSteg.py -r -b 2 -s soundfile -o outputfile
  ```
- [ffmpeg](https://ffmpeg.org/documentation.html) — Universal media converter. Check integrity of audio files.
  ```bash
  ffmpeg -v info -i stego.mp3 -f null -
  ```
- [Deepsound](http://jpinsoft.net/deepsound/download.aspx) — Hide and check for information encrypted with AES-265 in sound files.
  - If DeepSound finds any data hidden, you'll need to provide the password to unlock it.


## Software for Steganography
- [Gimp](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwj09LaF54yAAxUGITQIHeNiDm8QFnoECA4QAQ&url=https%3A%2F%2Fwww.gimp.org%2F&usg=AOvVaw14Av6K8pNdgfrkZATYVj-5&opi=89978449) — "GNU Image Manipulation Program," raster graphics editor used for image manipulation and editing, transcoding between image file formats, etc.
- [Stegsolve](https://wiki.bi0s.in/steganography/stegsolve/) — Analyze images in different planes by taking bits off the image.
  - Installation:
  ```bash
  wget https://github.com/eugenekolo/sec-tools/raw/master/stego/stegsolve/stegsolve/stegsolve.jar
  ```
  - Usage:
  ```bash
  java -jar stegsolve.jar
  ```

## Misc. and Other Resources
- [stego-toolkit](https://github.com/DominicBreuker/stego-toolkit) —  Docker image useful for solving CTF Steganography challenges. Includes nice descriptions of all the tools included.
- [Steganography Tools List](https://0xrick.github.io/lists/stego/) — List of useful tools and resources for steganography. Includes brief description of each.



# RSA Decryption Tools
---
- [Integer Factorization Calculator](https://www.alpertron.com.ar/ECM.HTM)
- [Prime Factorization Calculator](https://www.calculatorsoup.com/calculators/math/prime-factors.php)
- [RSA Calculator](https://www.cs.drexel.edu/~jpopyack/Courses/CSP/Fa17/notes/10.1_Cryptography/RSA_Express_EncryptDecrypt_v2.html)
- [dcode RSA Cipher Calculator](https://www.dcode.fr/rsa-cipher)
- [Carmichael Function Calculator](https://comnuan.com/cmnn02/cmnn02006/cmnn02006.php)
  


# Misc. Command Line Cryptography Tools
---
- [Ciphy](https://github.com/Ciphey/Ciphey) — Automatically determine cipher and output result.
- [RsaCtfTool](https://github.com/RsaCtfTool/RsaCtfTool) — Uncipher data from weak public keys and attempt to recover the corresponding private key.
- opencv-python (Find hidden content using Fast Fourier Transform (FFT))
