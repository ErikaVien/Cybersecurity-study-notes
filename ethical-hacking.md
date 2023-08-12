# Ethical Hacking Bootcamp 2023 : Zero to Mastery
### 5 stages of Penetration Testing
1. Information Gathering
2. Scanning
3. Exploitation
4. Maintaining Acess
5. Covering Tracks

## Information Gathering : finding username with Sherlocks
some tools may break and not works, so download other tools

git clone webaddress

if it a php, run the command : php RED_HAWK.php

if it a python, run the commad : python3 sherlock.phy

running missing module : pip3 install modulename

## Scanning

Firewall : monitor the monitor network traffic

IDS : intrusion detection system

filtered port : nmap cannot scan whether the port is open or close as there is firewall where packets were drop
**netdiscover** : scanning for IP in the network

arp -a  : scanning for IP in the network

netstat -nr > check the router IP
**TCP (transmission control protocol )**  send packets, check errors and resend packets

- request and respond packets

- download files

- 3 way handshake > SYN, SYN/ACK, ACK

**NMAP scanning**
-sn : no port scanning, only what host up

-sV : version scanning

-O : scan for what operational system : Linux, windows, etc

-sU : UDP scan

-sT :

-sS : SYN scan

-p : for port scanning > -p 80

to save the result to files : nmap 192.x.x.x >> results.txt  or   nmap -oN results.txt

**UDP (User Datagram protocol)**

- speed and error correction is not need

- steaming video and gaming

## Vulnerability Analysis
**Finding first vulnerability with Nmap scripts**:
nmap scripts: detect server vulnerability, brute force attacks, detect malware, collect information

usr/share/nmap/scripts
NMAP scripts categories : auth, speed, brute, default, broadcast, malware, vuln, banner, etc...

-F = 100 ports

> nmap --scripts categories/scripts_name IP

> sudo nmap  --scripts malware IP -sS -F

to login ftp port > ftp 192.x.x.x

**manual search for vulnerability analysis:**
- by searching the VERSION on google (mostly use)
> searchsploit VERSION-name (just copy and paste)

> locate path-name

> cd path-name(copy and paste)

## Exploitation and Gaining Excess
Shell = Payload - execute command and connect to target machine

reverse shell - connection to Kali Linux from listening to incoming connection target machine

binds shell - connection through opened ports of target machine. Useless as there is Firewall.

Firewall prevent target machine from opening ports.

### msfconsole

->nmap -sV  = scan version

->searchsploit version_name => searchsploit vsftpd 2.3.4

msf5 -> seach vsftpd

msf5 -> use exploit /unix/ftp/exploit_name

msf5 -> show info (for more info about the exploit)

msf5 -> show options (set up things, RHOSTS, etc)

msf5 -> set RHOSTS 192.168.x.x

msf5 -> show payloads

msf5 -> show targets

msf5 -> exploit

exit to exit

**Default credential router**
- checking IP gateway for router : netstat
- Website address = IP gateway

### SERVICE - bindshell
- NO Authentication
- misconfiguration - administrator set up without authentication, etc

use netcat (nc)

-> nc 192.168.x.x port_number

### SERVICE - telnet
- this vulnerability only possible due to information disclosure - as there username and password on the bannner of Metasploitable

-> searchsploit VERSION

to connect to telnet machine :

-> telnet 192.168.x.x

-> sudo su

### SERVICE - netbios-ssn -> samba

-> searchsploit samba

auxiliary module can sometime be scanner : can be use to scan for the version

msf5 -> search auxiliary

msf -> use auxiliary/scanner/smb/

msf5 -> show info

msf5c-> run

### brute force attack - SSH login
- create username list, password list using nano
- search for auxiliary module for ssh login

-> use auxiliary/scanner/ssh/ssh_login

msf5 -> set USER_FILE , PASS_FILE, RHOSTS

msf5 -> run

msf5 -> sessions

msf5 -> sessions -i 1

-> ssh msfadmin@192.x.x.x

weak credential

## Gaining Acess(Trojan,Virus,Payloads) :

**1. Generating basic payload with Msfvenom****
- Target with no vulnerability.
- msfvenom
- exploit through payloads with target execute themself using email, link, etc
- turn off real-time protection on windows
  
**2. Generating Powershell payload with Veil:**
>apt-get install veil

>viel

wine is a program allow to open windows files in Linux, make sure to have wine installed before using the BAT to ExeConverter.

UPX is more use for malicious program

**3. The FatRat payload creation:**
Payload creation tools : TheFatRat

- creating backdoor, etc

>git clone website

>fatrat

FUD : fully undetectable

set listener

**4. Hexieditor and Antiviruses:**
- Bypass antivirus
- how to FUD : coding your own payloads, using new payloads, change binary using hexeditor programming language for coding

hexeditor : changing binary for inessential things/text in hash

**5. Making payload open an Image:**

1. make icon file using png - convert icon.com

2. making the ico executable , create SFX archieve, SFX options : extract and update file,overwrite all file. browse , mode : hide all.

set up listener

>use exploit

## Post Exploitation
- scroll through files system, look for files.
- extract files, steal passwords,
- control network : gain access into intra network
- run a keylogger : catch password, messge, searching on net, etc

- upload file to target machine : meterpreter > upload Ratdoor.exe
