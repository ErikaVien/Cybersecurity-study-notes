# Chapter 11 : Installing and Upgrading Operating Systems
## Windows Editions and Features
- Windows 1.01
- Windows 3.11 : Network folder, Options, User Control, Minesweeper game
- WIndows 95 : desktop and start menu
- Windows 98 : new icon, pinball games
- Windows 2000
- Windows XP
- Windows 7
- Windows 8 : have live tiles
   
1. Search to see the Windows edition and version command : **Winver**
2. Windows update release frequently

#### Windows 10 
   - _RAM need 1GB for 32bit, 2GB for 64 bit_
1. **Windows 10 Single** - No Domain, No RDP, No Group Policy, No Bitlocker, No Long-Term Servicing Branch
2. **Windows 10 Pro**- Include all, except for Long-Term Servicing Branch
3. **Windows 10 Pro for Workstations** - Include all, except for Long-Term Servicing Branch
4. **Windows 10 Enterprise** - Include All,have Long-Term Servicing Branch: Update will be done only for certain interval, unless there major security to fix


#### Windows 11 
- require (Unified Extensible Firmware Interfaces)UEFI, must sure motherboard support UEFI
- requires enable Secure Boot and Trusted Platform Module (TPM) 2.0 on motherboards
- Zero Trust - need to verify on all stage
- must have internet connection to set up account
- not have local account
- X-Box features
- _Min 4GB RAM, Min CPU 1Ghz 2 cores_
1. **Windows 11 Home** - No Domain, No RDP, No Group Policy, No OneDrive for Business, No Bitlocker, No Long-Term Servicing Channel
2. **Windows 11 Pro** - Include all, except Long-Term Servicing
3. **Windows 11 Pro for Workstation**s - Include all, except Long-Term Servicing
4. **Windows 11 Enterprise** - Include all, have Long-Term Servicing

### Boot From Everything
1.**ISO image (Disk Image File)** : a perfect copy originally from optical media
- must be in partition in 
- can mount ISO file : just right click and choose mount
    - mount allow user to access the contents of ISO file
- can burn disc image to optical media
    - Tools : Rufus 
      - Rufus allow burn iso to be bootable thumb drive
      - Rufus allow burn into SD card to put in Resberry pie
- downside : windows on thumb drive with ISO in thumb drive
2. **Bootable over Network**
    - Pre-boot Execution Environment (PXE)
    - Apple NetBoot
  - System Setup -> over network -> Enter network address
3. **Windows Recovery Environment (WinRE)**
    - built in every copy of windows
    - A personal copy windows installation media
       - Control Panel -> Recovery -> Create a recovery drive
    - for troubleshoot when PC cannot start, etc
    - must have 16GB drive
## Installing and Upgrading Windows 10
### Install Windows 10 
- During installation
- can repair installation
- image deployment - can be done through remote network installation to remotely update many computers simultaneously
- End-of-Life (EOL) for OS occurs at the end of the product lifecycle
- In-place upgrade : performing an upgrade using built-in Windows OS installer

### Post-Installation Tasks
Tasks that need to do after installed Windows
1. Be sure to install third-party driver after installing or upgrade an OS
    - check error in Device Manager to ensure hardware properly installed
    - Optical Media come with motherboard
    - Search online for drivers or tools
    - Dont install extender web broswer
2. Windows Update - windows update, notification update, etc
3. Recovery disk/partition
    - must have 16GB flash drive
4. Create Restore Point : Snapshoots
    - System Properties -> turn on System Protection
    - create a restore point
5. Setting up anti-malware and firewall
    - Windows have pre-installed anti-malware, antivirus and firewall
6. File Histroy : automatic backup your files
## Installing and Updating Linux
1. Choose Distributions (distros or versions)
    - Ubuntu : great desktop version
    - download desktop iso
3. Installing
    - minimal installation
    - download update while installing
    - basic install : erase disk and install
4. Update Ubuntu Linux with Software Updater
    - at Start button -> Software updater

## Upgrading MacOS
1. MacOS upgrade can be found under Software Update
    - Apple button -> System Preferences -> System Update -> Upgrade Now
    - Agree all End-user License Agreement (EULA)
    - install in hard disk
    - then Restart
    - Be sure to check before upgrade as it can introduce incompatiblities or bugs in your work flow : _Dont upgrade immediately after a new update release!_
