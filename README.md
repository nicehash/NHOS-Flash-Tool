# NHOS Flash Tool
- [Introduction](#introduction)
- [Quick Setup](#setup)
- [NiceHash OS Configuration](#config)
- [Download NiceHash OS Flash Tool](#downloads)

# <a name="introduction"></a> Introduciton
NiceHash OS Flash Tool is __NiceHash OS image flasher__, which allows users to download, configure and flash image of NiceHash OS on
 their USB flash drive. It __automaticaly__ checks and __downloads__ latest NiceHash OS image if its not present on the system.
 
 # <a name="setup"></a> Quick setup
 NiceHash OS Flash Tool is available for __Linux__, __MacOs__ and __Windows__ operating systems. __No previous NiceHash OS image download is required!__  However if you already have latest NiceHash OS image downloaded on your system you can place it in NiceHash OS Flash Tool downloads folder and skip the downloading part.
 Quick setup as follows: 
 
 __WARNING:__
The process described below will delete any data currently on your flash drive. Make sure to back up your flash drive's data to another storage location before proceeding.

- Download and install NiceHash OS Flash Tool for your operating system.
- Insert USB flash drive and complete [configuration fields](#config).
- Start flashing.

 # <a name="config"></a> NiceHash OS Configuration
- __BTC Address:__ Your NiceHash BTC address. __**Mandatory*__
- __Worker name:__ Name of your mining machine (sometimes referred to as `rig name`). Have in mind, that `worker` name is limited to alphanumeric characters from English alphabet, `a` to `z`, `A` to `Z`, `0` to `9` and characters `-` (hyphen), `_` (underscore). After succesfull flashing it will automaticaly increment by 1 if the name ends with a number.
Optionaly `(%d)` or `(%d,n)`(n - start number) can be used anywhere in the name. `(%d)` will be replaced by 1 and increment with each succesfull flash, `(%d,n)` will be replaced with __number n__ and increment with each succesfull flash.__**Optional*__
- __Group name:__ Put your mining machine into group.__**Optional*__
- __Wireless ssid:__ Provide the name for a wireless network access.__**Optional*__
- __Wireless key:__ Security key for wireless network access authentication.__**Optional*__
- __SSH key:__ SSH public key for user authentication.__**Optional*__

 __Automatic worker name increment example:__
 Worker name can be incremented automaticaly if name ends with a number. Optionaly `(%d)` or `(%d,n)` can be used anywhere in the name to increment worker name number.
 - `worker_name10` equals  `worker_name10` in configuration file on flashed usb flash drive. The number will increment by 1 after each successful flash.
 - `worker_(%d)name` equals `worker_1name` in configuration file on flashed usb flash drive. The number will increment by 1 after each successful flash.
 - `worker_(%d,5)name` equals `worker_5name` in configuration file on flashed usb flash drive. The number will increment by 1 after each successful flash.
 - `(%d)worker_(%d,55)name` equals `1worker_55name` in configuration file on flashed usb flash drive. __Both__ numbers will increment by 1 after each successful flash.
 
 # <a name="downloads"></a>Download NiceHash OS Flash Tool
 - Download installer for Windows([32bit](https://github.com/nicehash/NHOS-Flash-Tool/releases/download/1.0.9/NHOS-Flash-Tool-1.0.9-win32.exe),[64bit](https://github.com/nicehash/NHOS-Flash-Tool/releases/download/1.0.7/NHOS-Flash-Tool-1.0.9-win64.exe))
 - Download installer for Linux([DEB](https://github.com/nicehash/NHOS-Flash-Tool/releases/download/1.0.9/NHOS-Flash-Tool-1.0.9.deb),[RPM](https://github.com/nicehash/NHOS-Flash-Tool/releases/download/1.0.9/NHOS-Flash-Tool-1.0.9.rpm))
 - Download installer for [MacOS (DMG)](https://github.com/nicehash/NHOS-Flash-Tool/releases/download/1.0.9/NHOS-Flash-Tool-1.0.9.dmg)
