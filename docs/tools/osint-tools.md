# Open Source Intelligence

## OSINT Web Resources
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

## Command Line OSINT Tools
- [ExifTool](https://exiftool.org/) — Meta information reader/writer
  - [File types and meta information formats supported by ExifTool](https://github.com/exiftool/exiftool)
  - `exiftool <filename>`
    
## OSINT Misc. Information and Resources
- [50 Common Ports You Should Know](https://www.geeksforgeeks.org/50-common-ports-you-should-know/#)
- [Service Name and Transport Protocol Port Number Registry](https://www.iana.org/assignments/service-names-port-numbers/service-names-port-numbers.xhtml) — IANA
- [Google Dork Cheatsheet](https://gist.github.com/sundowndev/283efaddbcf896ab405488330d1bbc06)
- [List of DNS Record Types](https://en.wikipedia.org/wiki/List_of_DNS_record_types)
- [Google Hacking Database](https://www.exploit-db.com/google-hacking-database)


## Scan Wi-Fi Network
### arp-scan
[arp-scan](https://www.kali.org/tools/arp-scan/) is a network scanning tool that uses the ARP protocol to discover and fingerprint IPv4 hosts on the local network. 

Send ARP requests to target hosts and display resources:
```bash
arp-scan [options] [hosts...]
```

Scan a subnet, specifying interface to use and a custom source MAC address:
```bash
arp-scan -I eth0 --srcaddr=DE:AD:BE:EF:CA:FE 192.168.86.0/24
```

### iwlist
```bash
iwlist <if> scanning | grep -A5 -B5 -E "AA.BB.CC.DD.EE.FF" | grep -i ESSID
```

### Misc
- [Kali - Hidden WiFi Network Name](https://kalitut.com/hidden-wifi-network-name/)
- mdk3
- Airodump-ng
- [Wigle.net User Reported Wireless Network Data](https://wigle.net/)
- [Article on wireless networking, wardriving, SSIDs, MAC addresses, and hotspots](https://www.osintcurio.us/2019/01/15/tracking-all-the-wifi-things/); includes basic walkthrough of [wigle.net](https://wigle.net/).


## Wi-Fi Terms and Definitions
**Wireless LAN (WLAN)** is a network in which devices are communicating wirelessly with each other in a defined area. 
It is ultimately connected to a wired network.

A **Wireless Access Point (WAP)** accepts a wireless signal from multiple devices and retransmits them to the rest of the network.

The **Service Set Identifier (SSID)**, also called the **"network name"** is the fundamental identification for an 802.11 **Wireless Local Area Network (WLAN)**, whcih includes both home networks and public hotspots.
The **SSID** is a case-sensitive text string that can contain letters, digits, or both, and has a maximum length of 32 characters. 
Wi-Fi units are preprogrammed by router manufacturers with a default **SSID** (examples: TP LINK, D LINK, JIO FI, or DEFAULT). 

The **Basic Service Set Identifier (BSSID)** is not the same as the **SSID**.
The **Basic Service Set (BSS)** is a group of wireless devices that work with the same **Access Point (AP)**. 
The **BSSID** is the **AP**'s physical **MAC address**. 
This info is included in the packets.

One **Service Set** can be extended by adding more **AP**s; this is called the **Extended Service Set (ESS)**. 
The shared network name is referred to as the **Extended Service Set Identifier (ESSID)**. 
Every **AP** broadcasts the same **SSID** to its users.

- WEP
- WPA/WPA2
- WPS
- WAP: Wireless Access Point







