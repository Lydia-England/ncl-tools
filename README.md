# NCL Tools and Resources
The [National Cyber League (NCL)](https://nationalcyberleague.org/) is a bi-annual, virtual, puzzle-based, capture-the-flag style cybersecurity competition for high school and undergraduate students. 

*From the [NCL About Page](https://nationalcyberleague.org/about):* "NCL offers a fun way to learn and apply your skills in a safe environment - but it’s so much more than that, because with their NCL Scouting Reports you can present credible proof to employers of your hands-on expertise."
An article from the Applied Cybersecurity Division at NIST describes the [National Cyber League NICE Framework Success Story](https://www.nist.gov/itl/applied-cybersecurity/nice/nice-framework-resource-center/nice-framework-success-story-national).  

Information on upcoming NCL Competitions can be found [here](https://nationalcyberleague.org/competition).


This is an unofficial, non-exhaustive list of tools I've found useful during the competition or that were recommended to me.

## Categories
- [**Open Source Intelligence**](/tools/osint-tools.md#Open-Source-Intelligence)
  - [OSINT Web Resources](/tools/osint-tools.md#OSINT-Web-Resources)
  - [Command Line OSINT Tools](/tools/osint-tools.md#Command-Line-OSINT-Tools)
  - [OSINT Misc. Information and Resources](/tools/osint-tools.md#OSINT-Misc.-Information-and-Resources)
- [**Cryptography**](/tools/cryptography-tools.md#Cryptography)
  - [Online Cipher Identification and Decryption Tools](/tools/cryptography-tools.md#Online-Cipher-Identification-and-Decryption-Tools)
  - [Online Steganography Tools](/tools/cryptography-tools.md#Online-Steganography-Tools)
  - [Online RSA Decryption Tools](/tools/cryptography-tools.md#Online-RSA-Decryption-Tools)
  - [Command Line Cryptography Tools](/tools/cryptography-tools.md#Command-Line-Cryptography-Tools)
  - [Cryptography Software](/tools/cryptography-tools.md#Cryptography-Software)
  - [Additional Resources](/tools/cryptography-tools.md#Additional-Resources)
- [**Password Cracking**](/tools/password-cracking-tools.md#Password-Cracking)
  - [Online Password Cracking Tools](/tools/password-cracking-tools.md#Online-Password-Cracking-Tools)
  - [Command Line Password Cracking Tools](/tools/password-cracking-tools.md#Command-Line-Password-Cracking-Tools)
  - [Hashcat](/tools/password-cracking-tools.md#Hashcat)
  - [Wordlists and Rule Lists](/tools/password-cracking-tools.md#Wordlists-and-Rule-Lists)
  - [Password Cracking Information and Resources](/tools/password-cracking-tools.md#Password-Cracking-Information-and-Resources)
- [**Log Analysis**](/tools/log-analysis-tools.md#Log-Analysis)
  - [Command Line Log Analysis Tools](/tools/log-analysis-tools.md#Command-Line-Log-Analysis-Tools)
  - [Creating Programs to do Log Analysis](/tools/log-analysis-tools.md#Creating-Programs-to-do-Log-Analysis)
- [Network Traffic Analysis](/tools/network-traffic-analysis-tools.md#Network-Traffic-Analysis)
  - [Command Line Network Traffic Analysis Tools](/tools/network-traffic-analysis-tools.md#Command-Line-Network-Traffic-Analysis)
  - [Network Traffic Analysis Resources and Information](/tools/network-traffic-analysis-tools.md#Network-Traffic-Analysis-Resources-and-Information)
- [**Forensics**](/tools/forensics-tools.md#Forensics)
  - [General Forensics Tools](/tools/forensics-tools.md#General-Forensics-Tools)
  - [Steganography Tools](/tools/forensics-tools.md#Steganography-Tools)
  - [Unzip, Extract Files](/tools/forensics-tools.md#Unzip,-Extract-Files)
  - [General Forensics Command Line Analysis Tools](/tools/forensics-tools.md#General-Forensics-Command-Line-Analysis-Tools)
  - [Disk Imaging, Log](/tools/forensics-tools.md#Disk-Imaging,-Log)
  - [Binwalk](/tools/forensics-tools.md#Binwalk)
  - [Forensics Resources and Information](/tools/forensics-tools.md#Forensics-Resources-and-Information)
- [**Wireless Access Exploitation**](/tools/wireless-access-exploit-tools.md#Wireless-Access-Exploitation)
  - [Graphical Wireless Access Exploitation Tools](/tools/wireless-access-exploit-tools.md#Graphical-Wireless-Access-Exploitation-Tools)
  - [Command Line Wireless Access Exploitation Tools](/tools/wireless-access-exploit-tools.md#Command-Line-Wireless-Access-Exploitation-Tools)
  - [Misc. Wireless Access Exploitation Tools](/tools/wireless-access-exploit-tools.md#Misc.-Wireless-Access-Exploitation-Tools)
- [**Scanning and Reconnaissance**](/tools/scanning-recon-tools.md#Scanning-and-Reconnaissance)
  - [Command Line Scanning and Reconnaissance Tools](/tools/scanning-recon-tools.md#Command-Line-Scanning-and-Reconnaissance-Tools)
  - [Graphical Scanning and Reconnaissance Tools](/tools/scanning-recon-tools.md#Graphical-Scanning-and-Reconnaissance-Tools)
  - [Nmap](/tools/scanning-recon-tools.md#Nmap)
- [**Web Application Exploitation**](/tools/web-app-exploit.md#Web-Application-Exploitation)
  - [Command Line Web Application Exploitation Tools](/tools/web-app-exploit.md#Command-Line-Web-Application-Exploitation-Tools)
- [**Enumeration and Exploitation**](/tools/enumeration-exploit-tools.md#Enumeration-and-Exploitation)
  - [General Enumeration and Exploitation Tools](/tools/enumeration-exploit-tools.md#General-Enumeration-and-Exploitation-Tools)
  - [Command Line Enumeration and Exploitation Tools](/tools/enumeration-exploit-tools.md#Command-Line-Enumeration-and-Exploitation-Tools)
  - [Enumeration and Exploitation Information and Resources](/tools/enumeration-exploit-tools.md#Enumeration-and-Exploitation-Information-and-Resources)
## Appendix
- Command Line Commands
- Environment
- Resources
- NCL Strategies


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

