# Chapter 9 : Implementing Mass Storage

## Redundant Array of Inexpensive Disk (RAID)
1. hardware : using dedicate controller or card, system setup or BIOS
2. software : through operating system, run software

**Speed and data redundance**
- RAID 0 - striping - speed - a document broken into pieces of data store alternatively into 2 drive
- RAID 1 - mirrored - redundancy - copying each data into 2 drive
- RAID 5 - parity - min 3 drive - 1+3=4, can loose up to 1 drive only
- RAID 6 - RAID5+RAID1 - can loose up to 2 drives
- RAID 10 - 4 drives - striping mirror - striping into 2 pairs of mirrored, cannot lose a pair mirrored drive
- RAID 0+1 -  4 drives - a pair of striping and then mirrored into 2 pair of striping

### Hardware RAID
- require a controller to configure the RAID arrays
- built-in RAID controller
- hardware RAID controller : dedicated expansion card
- can change regular hard-drive (AHCI) to RAID in it BIOS setting
- completed array(pool) looks like a single drive to the OS

### Software RAID
- no dedicate controller depends on CPU and OS
- OS handle the RAID, Windows can handle RAID 0 and RAID 1
1. Disk Management, right click, new mirrored volume or stripped volume
2. Storage Space, create a new pool and storage space
    - Resiliency type : Simple or Just a bunch of disks (JBOD), two-way mirror, three-way mirror, parity (RAID5)
    - can create a pool of two-way and parity, then create them into three-way mirror
  
### Encrypting Mass Storage (storage devices)

1. To encrypt a document, right-click, properties, advanced, encrypt contents to secure data
2. File-based encryption encrypt files and folders, disk-based encrypts entire drives
3. FileVault for MacOS
4. Windows used Encrypted File System(EFS) to encrypt folders and files
5. Windows used Bitlocker to encrypt entire hard drives
6. Trusted Platform Module (TPM) is a chip in motherboard
      - turn on TPM at system setup - security - trusted computing - security device support
      - turn on Bitlocker, back up your key
  
## Mass Storage Troubleshooting

**Three rule for mass storage**
1. Back it up
2. Mental reinstall
3. Triple check

### Troubleshooting
1. **RAID not found/not working** - right driver, system setup, controller active, power
2. **Read/write failure** :  Self-monitoring, Analysis and Reporting Technology (SMART) hard-drive, or replace hard-drive
3. **Slow performance** - need more RAM
4. **Loud clicking/grinding sound** : mechanical failure inside hard-drive - replace hard drive
5. **Failure to boot** - check boot order
6. **Drive not recognized/bootable device not found/missing drive**s - reformat drive
7. **OS not found** - boot process mess up , check system setup boot order
8. **Attempt to boot incorrect device** : check boot order
9. **Continuous reboot** : refer troubleshooting OS
10. **Mass storage device run on controller:** check RAID,USB, SATA controller
