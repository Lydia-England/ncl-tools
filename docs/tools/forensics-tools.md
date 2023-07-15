# Forensics

## General Forensics Tools
- [HexEd.it](https://hexed.it/) — Online hex editor
- [Autopsy Forensic Browser](https://www.kali.org/tools/autopsy/) — Digital forensics platform
  - [Autopsy Tutorial (blog post)](https://cryptokait.com/2021/03/08/digging-into-autopsy-forensics/)
- [pspy](https://github.com/DominicBreuker/pspy) — Low privilege process snooper.
- [Audacity](http://sourceforge.net/projects/audacity/) — Analyze sound files.

## Unzip, Extract Files
- [7-Zip](https://www.7-zip.org/) — File archiver with a high compression ratio (and opens just about anything)
- `unzip file.zip` to extract the archive file residing in the current directory and extract its contents also to the current directory. 
- `unzip file.zip -d dest_folder` to extract the zip file to another folder.
- `unzip filename.docx -d dest_folder` to unzip .docx files to see what's inside.
- `gzip -d file.gz` (or `gzip -dk file.gz` to keep compressed file) — Unzip `gz` File
- `gunzip file.gz` — Unzip `gz` file (this command is essentially an alias to `gzip -d`.
- `tar -xf archive.tar.gz` to extract a `tar.gz` file.
- `unrar` —
  
## General Forensics Command Line Analysis Tools
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

  
## Steganography
Note that many other steganography tools are detailed on the [Steganography page](/stego-tools.md)
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


## Generate hash from command line
- `sha256sum <datafile>` 
- `sha256sum /path/to/datafile > checksum` to generate the hash for a file in a directory. Use `cat` command to display the contents.


# File Extensions  (and what to try)

## .docx

## .tar.gz

## .zip

## .bin
The .bin extension is most commonly associated with compressed binary files. 
A BIN file is a generic data file that stores information entirely or partially in binary format. 
A BIN file may be an image or a video (think CD or DVD), or some other kind of executable.

Bin files are often used for distributing executable files for program installations; in this case, a .bin file is a self-extracting binary file for Linux and Unix-like operating systems. 
In this case, to extract and open a bin file:
- Make the file executable by using `chmod` command:
  ```bash
  chmod +x filename.bin
  ```
- Execute the file: 
  ```bash
  ./filename.bin
  ```

If the BIN file isn't executable, you can instead mount the file to a virtual drive.
Instructions for Linux systems can be found [in this article](https://ubunlog.com/en/que-es-un-archivo-bin-y-como-abrirlo-en-ubuntu/#Montar_el_BIN_como_disco_virtual).

Alternatively, you can convert the BIN file into an ISO file, which allows you to use many more programs to burn or mount it.
One popular program to do this is MagicISO.

Finally, if the above fail, you can extract the contents of the file using one of the following tools:
- bchunk
- acetoneiso
- ISO Furius
- Gmount-iso
- cdemu

## .log



