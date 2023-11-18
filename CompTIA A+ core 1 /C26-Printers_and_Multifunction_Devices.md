# Chapter 26 - Printers and Multifunction Devices
### Inkjet printer
- the ink when heated is shoot out shoot across paper, the cartridge move back and forth
- Inkjet colors：M, C, Y, K (black)
- Multifunction devices - scanner, printer, copier, Fax
- Maintenance : clean nozzle, calibration, replace cartridges, clear jams

### Impact printer
- print head, print ribbon, platens
- can replace print head, ribbons, keep it clean
- tractor feeds paper : paper with lines of holes each sides
- pin strike on ribbons, pin pop out the printhead
- does not need preheat process

### Thermal Printer
- used to print out e-receipts, point of sales system
- special thermal paper, sensitive to heat
- Maintenance : frequently replace paper, clean heating element - printhead, remove debris

### 3D printer
- heat thermal plastic (resin & filament)
- create 3D image, create slice file, preheat print elements, push filament through extruder, print onto print bed
- components : extruder, feed tube, filament, heat element, print bed
- program : Cura，etc

### Installing Local Printer

1. Local Printer setup
2. Cloud printing
3. Network printer setup via wireless or ethernet cable

**Local Printer setup**
- USB connection, serial connection used by thermal printer
- read manual
- check device manager when plug in with computer
- firmware update
- spooler store print jobs in order
- windows will check for local printer first then network printer then virtual printer

**Sharing printer**
- Printer properties, sharing, render print jobs on client computer act as print server
- Shared printer security
    - user administration can open spooler
- Share printer over network
- To access shared printer, add a printer then select the shared printer
- To create a share printer, give a share name and enable files and printer sharing


### Install Wireless Printer
**Wired connection protocol : Mac -  SLP, Windows - LLDP**

**Installing wireless printer**
- check utilities on website
- check network band, same network
- ad hoc network - SSID
- wired : Zeroconf - windows, Bonjour - Mac which broadcast to everyone
- wireless : Airprint for Mac

### Troubleshooting printers

1. **Unable to install printer** : due to administration
2. **No connectivity** : check network, DHCP, physically connection, reinstall
3. **Rollback device driver**
4. **Access denied** : need permission
5. **No image on printer display** : is it turn on, sleep mode, logout from administrative mode
6. **Paper problems** : check rollers
7. **Low memory errors** : printer use old RAM , reduce resolution or buy RAM
8. **Error code** : learn your printer error code on website or manual book
9. **Bad printout** :
    - Garbled letter : bad driver - reset it
    - vertical lines on page : laser printer foreign on optically sensitive roller - change toner cartridge
    - colour : dead ink, or driver issues
    - streak/specking : inkjet problem - maintenance mode
    - print blank page : thermal printer heating problem, primary corona for laser printer is dead
10. **Bad driver**
