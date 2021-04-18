# Wireless-For-Dell-Inspiron-3458
All about wifi and bluetooth support on Hackintosh and Compatible card for Dell Inspiron 3458

## Intel Wireless Card:
I recommended using the AC8xxx, AC9xxx, AX200 and AX201

For 3xxx and 7xxx it have some issue:
- AC3xxx : Bluetooth working fine BUT wifi speed is bad 
- AC7xxx : Wifi and bluetooth working fine BUT when you use both of them, the bluetooth will unstable (Audio broken)

Download kext: 

Wifi: https://github.com/OpenIntelWireless/itlwm

Bluetooth: https://github.com/OpenIntelWireless/IntelBluetoothFirmware

## Broadcom Wireless Card:
I recommended using DW1820a, DW1560, bcm943324PCIEBT2 and some other native Realmac Wireless Card

#### *But these is some problem:*

- DW1820a (BCM94350ZAE) have alot of version (CN-096JNT, CN-0VW3T3, CN-08PKF4, 00JT494 493 and even Chinese Fake version)

        +   Bluetooth maybe unstable, Random Frezze System and it does not support 
        +   Download File will make Bluetooth unstable
        +   Some machine need to Force 5Ghz to make it support 5Ghz
        +   Some machine when connect to 5Ghz wifi, the bluetooth will unstable
        +   The Firmware Bluetooth sometime will not apply right version to make it working smooth
        +   The BCM94350ZAE chipset doesn't support power management correctly in macOS so needs to be disabled via property injection
        +   Some machine need to cover Pin to make it running (Bluetooth maybe not working)
        +   This card working flawless on PC but the laptop maybe :b unknown issue can't solved

<img align="" src="https://user-images.githubusercontent.com/54585187/115137381-fea4b600-a04f-11eb-818a-ec40ac79d12b.png" width="600">

###### Mine are using CN-0VW3T3 version. It working fine (i guess) but some feature i have not test yet (5Ghz Band Wifi connect, Apple Watch Unlock)

- bcm943324PCIEBT2: 

          + Some Wireless card will not support BT4.0 and stuck BT2.1 (also Continuty Feature not working too)
          + No Kext needed on High Sierra and under (With Mojave and Higher need AirportBrcmFixup.kext and maybe on BigSur not support)

<img align="" src="https://user-images.githubusercontent.com/54585187/115137266-61498200-a04f-11eb-8c8a-e03ce1c02c50.JPG" width="600">
<img align="" src="https://user-images.githubusercontent.com/54585187/115137306-9fdf3c80-a04f-11eb-829c-94b934622e9b.JPG" width="600">

Download Kext: 

- Wifi: https://github.com/acidanthera/AirportBrcmFixup/releases
- Bluetooth: https://github.com/acidanthera/BrcmPatchRAM/releases
- Extra: https://github.com/acidanthera/BT4LEContinuityFixup

## Atheros Wireless Card:

(I do not recommended this at all duel to Community Supoort and some card natively macOS but it too OLD)

# About M.2 Wireless Card Slot on Dell inspiron 3458
--Update soon--
