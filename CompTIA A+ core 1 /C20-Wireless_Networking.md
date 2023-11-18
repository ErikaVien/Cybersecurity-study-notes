# Chapter 20 : Wireless Networking

## Wireless Network Hardware
1. **IEEE 802.11** - standard wireless, build in in mobile

infrastruture mode

2. **wireless access point (WAP)** act as a bridge between internet network

3. **home router** - only 1 Ethernet connection

4. **wireless network card** - PCI

Service-set Identifier (SSID) : you look for wireless network to connect to

5. **Ad hoc mod** - no wireless access point, threat your system as wireless access point

6. **Antennas**:
   - omni-directional(like a stick with fuzzing ball), dipole :use for wireless ,
   - patch
   - highly directional : Yagi , like an old tv antenna, parabolic

## Wi-Fi standards
_**Wireless Access Point must be compatible with the device**_

1）802.11 base on Industrial, scientific and medical (ISM) radio bands: 

2）frequencies : 2.4GHz & 5GHz band

3）2.4GHz bands: 2.412-2.484: have 14 Channels

4）5GHz bands : 5.10GHz-5.875GHz :  up to 165 channels

5）802.11 extension :
  - 802.11a - 54Mbps - 5GHz
  - 802.11b - 11Mbps - 2.4GHz
  - 802.11g - 54Mbps - 2.4GHz : compatible with 802.11b  inside WAP is a radio
  - 802.11n (Wi-Fi 4)- 150Mbps - run on both 2.4GHz & 5GHz : MIMO (multiple in/multiple out) can allow signal Wireless Access Point to use multiple antenna to change radiation signal
  - 802.11ac(Wi-Fi 5) - 2.4GHz & 5GHz : Multiuser MIMO

## Wireless Mesh Network (WMN)

- great wireless solution for SOHO environments
- have base station and beacon devices that connect to base station
- mesh network use their own encryption
- ad hoc mode on steroid
- easy to configure, SSID
- robust

## Enterprise Wireless

- dedicate wireless access points, no AC adaptor, 
- use Power over Ethernet (POE) : electricity over ethernet cable
  - PoE switch, PoE injector
  - PoE+ have more electricity
- SSID , encryption, WPA,WPA2
- AAA - Authorization, Authentication, Accounting
- use RADIUS or TACACS+
    - RADIUS for network access authentication
    - TACACS+ for device administration   
- ESSID (Extended SSID) : same SSID on web on LAN

## Beyond Wi-Fi

1. Radio Frequency Identifier (RFID) - use on sticker, need reader to active, slow transmit
   - have Near Field Communication (NFC) : tap-to-print, tap-to-pay

2. Bluetooth : Personal Area Network (PAN) : some require PIN code
   - Class 1 : 100m range
   - Class2 : 10m range
   - Class 3 : less than 10m range
  
## Troubleshooting Wireless Connections

**Wi-Fi analyzer - helpful for diagnose wireless network, downloadable for mobile**
1. No connectivity :
      - SSID not exist
      - low Radio Frequency (RF) signal
      - get closer to SSID, look at the athenna
      - SSID broadcast turn off:  need WPA , Passcode

2. Limited or slow connectivity : external interference like a wall, microwave, baby monitor need to be move
3. Intermittent connectivity : low RF signal, too many ppl on your wireless network

