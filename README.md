> :warning: **Don't clone this efi.** [Download link](https://github.com/sohagmahin/Gigabyte-B360-Aorus-Gaming-3-Hackintosh/releases).
# Gigabyte-B360-Aorus-Gaming-3-Hackintosh
### Currently Running On MacOS BigSur(20B50)
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

## Change Serial,MLB,SMUUID

At first download GenSMBIOS tool from [here.](https://github.com/corpnewt/GenSMBIOS)

Then extract the file & click-> GenSMBIOS.command

#### 1 Select option :3
![](https://github.com/sohagmahin/Gigabyte-B360-Aorus-Gaming-3-Hackintosh/blob/main/screenshots/1.png "1. Select option :3")
#### 2 type: iMac19,2
![](https://github.com/sohagmahin/Gigabyte-B360-Aorus-Gaming-3-Hackintosh/blob/main/screenshots/2.png)

#### 3 Copy the Serial, Board Serial & SmUUID
![](https://github.com/sohagmahin/Gigabyte-B360-Aorus-Gaming-3-Hackintosh/blob/main/screenshots/3.png)

### 4 Open EFI->OC->config.plist then Replace it with your generated SMBIOS
```
Serial -> SystemSerialNumber
Board Serila -> MLB
SmUUID ->SystemUUID
```
![](https://github.com/sohagmahin/Gigabyte-B360-Aorus-Gaming-3-Hackintosh/blob/main/screenshots/4.png)

## Documentation<br>
* [Open Core Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)
## Credit<br>
* - Thanks to [Acidanthera](https://github.com/acidanthera) for providing [AppleALC](https://github.com/acidanthera/AppleALC), [HibernationFixup](https://github.com/acidanthera/HibernationFixup), [Lilu](https://github.com/acidanthera/Lilu), [NVMeFix](https://github.com/acidanthera/NVMeFix), [OcBinaryData](https://github.com/acidanthera/OcBinaryData), [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg), [RestrictEvents](https://github.com/acidanthera/RestrictEvents), [VirtualSMC](https://github.com/acidanthera/VirtualSMC), [VoodooInput](https://github.com/acidanthera/VoodooInput), [VoodooPS2](https://github.com/acidanthera/VoodooPS2), and [WhateverGreen](https://github.com/acidanthera/WhateverGreen).
