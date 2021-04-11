# Hackintosh Gigabye Z370N - Wifi
A hackintosh and mini itx build by me

Tested with lastest macos version (11.2.3)

# Specification 

```
Motherboard: GIGABYTE H370N Wifi
CPU: Intel® Core™ i7 6700
Ram: 16gb (2x8GB - 2666) CRUCIAL Ballistix Sport LT
VGA: MSI Radeon RX 560 Aero ITX
SSD: Western Digital Blue SN550 500GB PCIe Gen3 x4 NVMe
Wifi: bcm94360cs2
PSU: FSP Dagger Pro 600W
CPU Cooler: Noctua L12s
Case: Aklla A3
```

# OpenCore(0.6.8)

- https://dortania.github.io/OpenCore-Install-Guide/

# Installation

## Bios setup
```
Initial Display Output -> PCIe 1 Slot

DVMT Pre-Allocated -> 64MB

DVMT Total Gfx Mem -> 128MB

Above 4G decoding -> Enable

EHCI/XHCI Hand-off -> Enable

VT-d -> disabled

Wake on LAN Enable -> Disabled

CSM -> Disabled
```
## Make Usb bootable
```
sudo /Applications/Install\ macOS\ Big\ Sur.app/Contents/Resources/createinstallmedia --volume /Volumes/MyVolume
```

## Mount  and copy This EFI folder into EFI Partition
Using Drop EFI
[https://github.com/chris1111/Drop-EFI]
GenSMBOS
[https://github.com/corpnewt/GenSMBIOS]

```
git clone https://github.com/corpnewt/GenSMBIOS
cd GenSMBIOS
chmod +x GenSMBIOS.command
```
Copy EFI into EFI Partition on USB Installer

## Post Install
    
# Result
![big sur](./z370.png)

# Credit

- Apple for MacOS
- Dortania for Opencore Boothloader
- chris1111 for Drop EFI
- corpnewt for GenSMBIOS

