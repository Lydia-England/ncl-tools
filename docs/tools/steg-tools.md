# Steganography Tools

*Note: Many important Forensics tools also apply to cryptography (especially steganography) challenges. If you're stuck, check the [Forensics Tools page](/forensics-tools.md#Forensics).*

## Extracting data from all files
These are described more thoroughly in [Forensics Tools page](/forensics-tools.md#Forensics).
- Binwalk
- Foremost
- Exiftool
- Exiv2
- File
- Strings
- cmp (Comparison)


## Online Steganography Tools
- [TinEye](https://tineye.com/)
  - Reverse Image Search online.
- [StegOnline](https://stegonline.georgeom.net/upload) 
  - Online Steg Decoder
- [FotoForensics](https://fotoforensics.com/analysis.php?id=b4727b6206fb898a6ae76ea14d8d6ae4fc623752.110213)
  - Supported formats: **JPEG**, **PNG**, **WebP**, **HEIC**, and **AVIF**.
  - The "Hidden Pixels" analysis option is particularly useful.
- [Stegano](https://futureboy.us/stegano/) 
  - Supported formats: **JPEG**, **WAV**, **AU**.
  - Steghide online
- [Online Exiftool](https://exif.tools/) 
  - Online file metadata extraction
- [inlite](https://online-barcode-reader.inliteresearch.com/) 
  - QR Code, Barcode, Data Matrix, Driver License reader
- [Image to Binary Converter (dcode)](https://www.dcode.fr/binary-image) 
  - dCode tool that's potentially useful for stego in QR codes
- [Image Error Level Analyser](https://29a.ch/sandbox/2012/imageerrorlevelanalysis/) 
  - Identify manipulations to compressed (JPEG) images by detecting distribution of error introduced after resaving the image at a specific compression rate.
- [Magic Eye Solver/Viewer](http://magiceye.ecksdee.co.uk/) 
  - View hidden image (magic eye) 
  - includes slider to move towards/away from the magic eye.
- [Twitter Secret Messages](https://holloway.nz/steg/) 
  - Hide/extract secret messages in tweets (or any text) with *steg-of-the-dump.js*.
- [Hidden data in spaces](https://www.irongeek.com/i.php?page=security/unicode-steganography-homoglyph-encoder)


## Command Line Stego Tools
- [Identify](https://linux.die.net/man/1/identify) 
  - Describes format and characteristics of one or more image files.
  - Reports if an image is incomplete or corrupt. 
  - Member of the [imagemagick](https://linux.die.net/man/1/imagemagick) suite of tools.
- [Steghide](https://www.kali.org/tools/steghide/) 
  - Supported formats: **JPEG**, **BMP**, **WAV**, **AU**
- stegoVeritas (described below)
- [Zsteg](https://github.com/zed-0xff/zsteg) 
  - Supported formats: **PNG**, **BMP**
  - Detect stegano-hidden data in PNG and BMP.
  - Useful commands:
    - `zsteg -a file` Runs every detection method on the given file.
    - `zsteg -E payload file` Extracts data with the given payload (example" `b4,bgr,msb,xy`") 
- [Stegpy](https://github.com/dhsdshdhk/stegpy) 
  - Supported formats: **PNG**, **BMP**, **GIF**, **WebP**, **WAV**
  - Encoding information in image, audio files.
- [Pngcheck](http://www.libpng.org/pub/png/apps/pngcheck.html) 
  - Get details on a PNG file (or find out if it's actually something else).


## stegoVeritas
[stegoVeritas](https://github.com/bannsec/stegoVeritas/) is "yet another Stego tool".
- Supported formats: **JPG**, **PNG**, **GIF**, **TIFF**, **BMP**
- Will attempt to run on any file.

Usage:
```bash
stegoveritas [optional args] file
```

(Some of the) useful image options:
- `-bruteLSB` to attempt to brute force any LSB related steganography.
- `-meta` to check file for metadata information
- `-extractLSB` to extract a specific LSB RGB from the image. 
  - Use with `-red`, `-green`, `-blue`, and `-alpha`.
- `-trailing` to check for trailing data on the given file.
- `-steghide` to check for StegHide hidden info.

Multi options:
- `-exif` to check this file for exif information.
- `-xmp` to check this file for xmp information.
- `-carve` to attempt to carve/extract things from this file.



## Fast Fouier Transform (FFT) Steganography Tools
- [Imaging Web Demo - FFT Tool](http://bigwww.epfl.ch/demo/ip/demos/FFT/) 
  - Online FFT Tool
- [Ejectamenta](https://www.ejectamenta.com/Fourifier-fullscreen/) 
  - Online FFT Tool
- [FFTStegPic](https://github.com/0xcomposure/FFTStegPic) 
  - Python script for digital image stego with FFT.
- opencv-python 
  - Find hidden content using Fast Fourier Transform (FFT).


## Audio and Video Steganography Tools
- [Sonic Visualizer](https://www.sonicvisualiser.org/) 
  - Visualization, analysis, and annotation of music audio recordings.
  - If you're stuck, always check the spectrogram of the audio.
- [Sonic Lineup](https://www.sonicvisualiser.org/sonic-lineup/index.html) 
  - Rapid visualisation of multiple audio files containing versions of the same source material. Part of the Sonic Visualizer family of applications.
- [Sonic Annotator](https://vamp-plugins.org/sonic-annotator/) 
  - Batch tool for feature extraction and annotation of audio files using [Vamp plugins](https://vamp-plugins.org/index.html). Part of the Sonic Visualizer family of applications.
- [Detect DTMF Tones (file upload)](http://dialabc.com/sound/detect/index.html) 
- [Detect DTMF Tones (demo)](https://unframework.github.io/dtmf-detect/) 
- [Wavsteg](https://github.com/ragibson/Steganography#WavSteg) 
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
- [ffmpeg](https://ffmpeg.org/documentation.html) 
  - Universal media converter. Check integrity of audio files.
  ```bash
  ffmpeg -v info -i stego.mp3 -f null -
  ```
- [Deepsound](http://jpinsoft.net/deepsound/download.aspx) 
  - Hide and check for information encrypted with AES-265 in sound files.
  - If DeepSound finds any data hidden, you'll need to provide the password to unlock it.
- [Online Audio Spectrum Analyzer](https://academo.org/demos/spectrum-analyzer/)


## Software for Steganography
- [Gimp](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwj09LaF54yAAxUGITQIHeNiDm8QFnoECA4QAQ&url=https%3A%2F%2Fwww.gimp.org%2F&usg=AOvVaw14Av6K8pNdgfrkZATYVj-5&opi=89978449)
  - "GNU Image Manipulation Program," raster graphics editor used for image manipulation and editing, transcoding between image file formats, etc.
- [Stegsolve](https://wiki.bi0s.in/steganography/stegsolve/) 
  - Analyze images in different planes by taking bits off the image.
  - Installation:
  ```bash
  wget https://github.com/eugenekolo/sec-tools/raw/master/stego/stegsolve/stegsolve/stegsolve.jar
  ```
  - Usage:
  ```bash
  java -jar stegsolve.jar
  ```
- [Imagemagick](https://imagemagick.org/index.php)
  - Supported formats: **JPEG**, **PNG**, **GIF**, **TIFF**, **PDF**,
  - Used for editing and manipulating digital images.
  - Can be used to create, edit, compose, or convert bitmap images.


## Misc. and Other Steganography Resources
- [stego-toolkit](https://github.com/DominicBreuker/stego-toolkit) 
  - Docker image useful for solving CTF Steganography challenges. Includes nice descriptions of all the tools included.
- [Steganography Tools List](https://0xrick.github.io/lists/stego/) 
  - List of useful tools and resources for steganography. Includes brief description of each.
- [Steganography Playbook](https://fareedfauzi.gitbook.io/ctf-playbook/steganography)
  - List of steps to take and tools to use, given different file types.


## Steganography Encryption Tools and Tutorials
Understanding the process of hiding information makes locating and extract information much easier. 
- [How to Hide Files Inside Images in Linux (article)](https://www.makeuseof.com/tag/hide-files-inside-images-linux/)
- [How to Create Steganography Challenges](https://cyberpj.medium.com/how-create-steganography-challenges-13-e32ce96aa7df)


---

