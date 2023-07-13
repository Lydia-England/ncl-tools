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
- Binwalk — Search a binary image for embedded files, executable code (described below). 
- [Foremost](https://tools.kali.org/forensics/foremost) — May catch something Binwalk misses.
- [steghide](https://github.com/StefanoDeVuono/steghide) — Hides and extracts data from files.
- zsteg — Find steganography in PNG and BMP files. 
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
