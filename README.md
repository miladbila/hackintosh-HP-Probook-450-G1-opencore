# hackintosh-HP-Probook-450-G1-opencore
![photo_2022-02-24_09-34-51](https://user-images.githubusercontent.com/53270843/155498903-72b48a62-86cd-42e3-a8c9-df36cf3c8307.jpg)
![photo_2022-02-24_09-34-57](https://user-images.githubusercontent.com/53270843/155498911-169c0497-4669-4a2c-b255-985a17813085.jpg)


## Specifications


| Specifications      | Detail                                      |
| --------------------|-------------------------------------------- |
| Model               | HP ProBook 450 G1                           |
| CPU                 | Intel Core i5-4200M                         |
| RAM                 | 8 GB 1600MHz DDR3                           |
| Integrated Graphics | Intel® HD Graphics 4600                     |
| Dedicated Graphics  | AMD Radeon 8750M 1GB                        |
| Monitor             | HD 1366*768 (15.6 inch)                     |
| Wireless Card       | Mediatek MT7630E 802.11bgn                  |
| Ethernet/LAN        | Realtek RTL8168/8111 PCI-E Gigabit Ethernet |
| Sound Card          | IDT 92HD91                                  |

## Working
- CPU Power Management
- IGPU Power Management
- Battery Status / Time
- Ethernet LAN
- Realtek Audio
- Audio Speaker/Mic Jack
- Keyboard & Media/Function Keys
- Trackpad & Gestures support
- USB 2.0 ports
- HP Webcam
- Sleep/Wakeup & Instant Wake
- Screen Brightness
- And pretty much everything not listed below
- Apple GUC firmware

## Not Working
- Dedicated GPU (Disabled in SSDT)
- USB 3.0 ports (I dont have any usb 3.0 device to remap for now)
- Wi-Fi & Bluetooth (There is no driver for mediatek PCI wifi/bluetooth)
- SDXC Card Reader (Not supported in MacOS)

## Not Tested
- HDMI Port (I'll test later)
- Screen LID sleep (my laptop LID sensor doesn't working if someone test that option tell me)

## OpenCore
- OpenCore v0.7.8 Release on Feb 07 2022

## ACPI Patch list
- SSDT-dGPU-Off : Disables Dedicated GPU (Optimus Method)
- SSDT-EC : Embedded Controller fix
- SSDT-LANC : Instant wake fix
- SSDT-PLUG : Power Management Fix
- SSDT-PNLF : Brightness Fix
- SSDT-HPET : IRQ fix
