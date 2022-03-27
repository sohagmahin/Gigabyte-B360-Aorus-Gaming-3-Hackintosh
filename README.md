[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)

> :warning: **Don't clone. How to get the EFI?.** [Download it from Releases](https://github.com/sohagmahin/Gigabyte-B360-Aorus-Gaming-3-Hackintosh/releases).

# Gigabyte-B360-Aorus-Gaming-3-Hackintosh

### Currently Running On MacOS Monterey 12.0.1 (21A559)

![](https://github.com/sohagmahin/Gigabyte-B360-Aorus-Gaming-3-Hackintosh/blob/main/screenshots/specs.png)

## Specs

```
Motherboard : Gigabyte B360 Aorus Gaming 3

Processor : Intel Core i7-8700 (6 core, 12 Threat)

Ram: GSkill 16GB DDR4

SSD : Samsung evo 860  250GB SATA

Graphics : Intel UHD 630 Graphics

Audio codec : Realtek® ALC892 (Layout-id : 1)

Ethernet : Intel I219V7 PCI Express Gigabit- Ethernet
```

## BIOS Setting

### BIOS Version: F15b

### Disable

```
* Fast Boot
* Secure Boot
* Serial/COM Port
* VT-d
* CFG Lock (must be disable)
* Intel Platform Trust

```

### Enable

```
* Above 4G decoding
* Hyper-Threading
* EHCI/XHCI Hand-off
* DVMT Pre-Allocated(iGPU Memory): 64MB
* SATA Mode: AHCI
```

## Change Serial,MLB,SMUUID

At first download GenSMBIOS tool from [here.](https://github.com/corpnewt/GenSMBIOS)

Then extract it & Open-> GenSMBIOS.command

#### 1. Select option :3

![](https://github.com/sohagmahin/Gigabyte-B360-Aorus-Gaming-3-Hackintosh/blob/main/screenshots/1.png "1. Select option :3")

#### 2. type: iMac19,2

![](https://github.com/sohagmahin/Gigabyte-B360-Aorus-Gaming-3-Hackintosh/blob/main/screenshots/2.png)

#### 3. Copy the Serial, Board Serial & SmUUID

![](https://github.com/sohagmahin/Gigabyte-B360-Aorus-Gaming-3-Hackintosh/blob/main/screenshots/3.png)

#### 4. Open EFI->OC->config.plist then Replace it with your generated SMBIOS

```
Serial -> SystemSerialNumber
Board Serila -> MLB
SmUUID ->SystemUUID
```

![](https://github.com/sohagmahin/Gigabyte-B360-Aorus-Gaming-3-Hackintosh/blob/main/screenshots/4.png)

## Guide<br>

- [Open Core Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)

## Credit<br>

- - Thanks to [Acidanthera](https://github.com/acidanthera) for providing [AppleALC](https://github.com/acidanthera/AppleALC), [HibernationFixup](https://github.com/acidanthera/HibernationFixup), [Lilu](https://github.com/acidanthera/Lilu), [NVMeFix](https://github.com/acidanthera/NVMeFix), [OcBinaryData](https://github.com/acidanthera/OcBinaryData), [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg), [RestrictEvents](https://github.com/acidanthera/RestrictEvents), [VirtualSMC](https://github.com/acidanthera/VirtualSMC), [VoodooInput](https://github.com/acidanthera/VoodooInput), [VoodooPS2](https://github.com/acidanthera/VoodooPS2), and [WhateverGreen](https://github.com/acidanthera/WhateverGreen).


[![Licence](https://img.shields.io/github/license/Ileriayo/markdown-badges?style=for-the-badge)](./LICENSE)
