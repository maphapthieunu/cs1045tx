# OpenCore Bootloader EFI cho máy HP Pavilion 15-cs1045tx

### Downloads
GitHub Releases: https://github.com/xnplz/cs1045tx/releases/tag/efi  
Google Drive: https://drive.google.com/file/d/1CdTwS9LAAOGsSJ7IzZXRtwHBkqkh_--1/view?usp=sharing  
Lưu ý: Cần sử dụng [7-Zip](https://7zip.org) hoặc phần mềm hỗ trợ giải nén file 7z.

### Spectifications
| Bộ phận | Tên | Hỗ trợ |
| ------- | --- | ------ |
| CPU | Intel Core i5-8265U | native |
| GPU onboard | Intel UHD Graphics 620 | native |
| GPU rời | NVIDIA GeForce MX130 | không dùng được, Apple có hỗ trợ GPU NVIDIA đời mới méo đâu |
| SSD M2 NVMe | Kingmax PCIe SSD 128GB | native |
| HDD | TOSHIBA MQ04ABF100 | cần kext [SATAUnsupported](https://github.com/khronokernel/Legacy-Kexts/blob/master/Injectors/Zip/SATA-unsupported.kext.zip) vì HP ngu |
| Card ethernet | Realtek RTL8168H | cần kext [RealtekRTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X/) |
| Card wifi | Intel Wireless-AC 9461 | cần kext của bên [OpenIntelWireless](https://github.com/OpenIntelWireless) (1) |

### Notes
(1): Wifi cần combo [itlwm](https://github.com/OpenIntelWireless/itlwm) + [HeliPort](https://github.com/OpenIntelWireless/HeliPort) hoặc [AirportItlwm](https://github.com/OpenIntelWireless/itlwm), hình như méo hỗ trợ AirDrop, Bluetooth cần [IntelBluetoothFirmware](https://github.com/OpenIntelWireless/IntelBluetoothFirmware)  
(2): Boot vào recovery thì gặp quả `[EB|#LOG:EXITBS:START]`, đang nhờ người investigate

### Thanks
1. [HP](https://www.hp.com/vn-vi/home.html): Wow I love this laptop
2. [Dortania](https://github.com/dortania): for their [guide](https://dortania.github.io/OpenCore-Install-Guide)
3. [QuanTrieuPCYT](https://github.com/quantrieupcyt): owner thicc smp dep trai, thanks for helping me much
4. [Krisbane](https://github.com/krisbane): ui chi meo simmy, also thanks for helping me much

ncct
