# OpenCore EFI for HP EliteDesk 800 G6 (i5-10500T)

EFI Folder for installing macOS on **HP EliteDesk 800 G6 Desktop Mini Business PC** using **OpenCore v1.0.4**.

---

## System Configuration

| Component        | Description                                       |
|------------------|---------------------------------------------------|
| **Model**        | HP EliteDesk 800 G6 Desktop Mini                 |
| **CPU**          | Intel® Core™ i5-10500T (6C/12T)                  |
| **iGPU**         | Intel® UHD Graphics 630                          |
| **SSD**          | KIOXIA 256GB XG6 NVMe PCIe Gen3 x4 (M.2 2280)    |
| **Ethernet**     | Intel® I219-LM 1 Gigabit Network (vPro)          |
| **Wi-Fi + BT**   | Intel® Wi-Fi 6 AX201 + Bluetooth 5.2             |
| **Audio**        | Realtek ALC3867                                  |
| **OpenCore**     | Version 1.0.4                                     |
| **Kexts Date**   | Updated until 04/04/2025                          |

---

## What's Working

- GPU acceleration (UHD 630)
- Audio (ALC3867)
- Bluetooth (AX201)
- Wi-Fi (AX201)
- All USB ports
- Secure Boot
- Sleep/Wake

---

## What's Not Working

You Tell Me :) 

**everything essential is working**.

---

## BIOS Settings

Before starting the installation, make sure to configure the BIOS as follows:

| Path                                                       Desired   
|--------------------------------------------------------  ------------
| Security > Secure Boot Configuration > Secure Boot      **Disabled** 
| Advanced > Boot Options > Fast Boot                     **Disabled** 
| Advanced > Built-In Device Options > Wake on WLAN       **Disabled** 
| Advanced > Power Management Options > PCIe Power Mgmt   **Disabled** 
| Advanced > Boot Options > Video Memory Size               **64MB**     

---

## Installation Guide

> **Reference**: [Dortania's OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)

### Preferred Method: Offline Installer

I recommend using an offline macOS installer generator:

- [UnPlugged by CorpNewt](https://github.com/corpnewt/UnPlugged)

This simplifies creating a bootable USB installer without internet dependency.

---

## Notes

- Make sure to generate your own SMBIOS using [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS).
- This EFI is based on the Macmini8,1 SMBIOS.

