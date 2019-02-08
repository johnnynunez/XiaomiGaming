# I'm a Student Engineering, life and my university career is expensive and work is hard. My repositories are free, please, reward me. Thank you
# [Reward me](https://www.paypal.me/johnnync13)<br />
# Xiaomi Mi Laptop Gaming" 2018

SUPPORT: Only Mojave<br />
CPU: I7-8750h <br />

1. Tutorial <br />
NVIDIA Optimus isn't compatible with MacOS so you will only be able to use the NVIDIA GPU not the Intel. Intel Wi-Fi isn't compatible with MacOS so to have wi-fi you need to buy a compatible Wi-Fi USB Adapter.

2. NVIDIA GPU <br />
If you want enable nvidia gpu, remove -wegnoegpu on Boot arguments.
2. NVIDIA GPU Drivers <br />
After installing the wi-fi and restarting your Mac you need to install the Nvidia Web Drivers, for that the easiest way is to use a handy patcher made by Benjamin Dobell (https://github.com/Benjamin-Dobell/nvidia-update)

Just open terminal and type: bash <(curl -s https://raw.githubusercontent.com/Benjamin-Dobell/nvidia-update/master/nvidia-update.sh)

This will find the best version, download and install it for you. Once installed, restart the computer

Troubleshoot in case the NVIDIA Web Drivers installation gives an error saying that your OS is not compatible:
You will need to do a few tweaks to make it work:
1) Check what is the latest supported OS code for that Web Driver
2) Open you SystemVersion.plist file inside CoreServices (FIND IT) and tweak your OS Code to match the NVIDIA one (make a backup first)
3) Install the Web Driver and don't restart
4) Go to /Library/Extensions and open the package contents of NVDAStartup.kext
5) Tweak info.plist to the OS Code of your OS
6) Now revert the Systemversion tweak back to the original version that you made a backup
7) Use RepairPermissions to repair the permissions fo the kext
8) Open the Nvidia Driver Managet tool and enable the NVIDA Web Driver - if not available restart your computer and then enable it.
8) Restart your computer



3. What's Working <br />
Native power management <br />
Intel GPU <br />
Audio (AppleALC) <br />
TrackPad <br />
HDMI video and audio <br />
Bluetooth <br />
USB 3.0 <br />
Brightness key <br />
Usb speed <br />
Built-in camera <br />
Built-in mic <br />
3. What's Not Working <br />
Wifi Intel <br />
## Credits

- [stevezhengshiqi](https://github.com/stevezhengshiqi) He is a good developer. I'm learning a lot about how to patch problems. Thanks for PCIList.aml and more.

- [RehabMan](https://github.com/RehabMan) Updated [OS-X-Clover-Laptop-Config](https://github.com/RehabMan/OS-X-Clover-Laptop-Config) and [Laptop-DSDT-Patch](https://github.com/RehabMan/Laptop-DSDT-Patch) and [OS-X-USB-Inject-All](https://github.com/RehabMan/OS-X-USB-Inject-All) for maintenance

- [vit9696](https://github.com/vit9696) Updated [Lilu](https://github.com/vit9696/Lilu) and [AppleALC](https://github.com/vit9696/AppleALC) and [WhateverGreen](https://github.com/vit9696/WhateverGreen)  for maintenance

- [alexandred](https://github.com/alexandred) Updated [Voodooi2c](https://github.com/alexandred/VoodooI2C) for maintenance
