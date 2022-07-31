## 1. Prerequisites

* Raspberry Pi Pico ([Amazon](https://amzn.to/3JbIsMw), [AliExpress](https://s.click.aliexpress.com/e/_DkGpnTv))
* SD Gecko/WiiSD ([Amazon](https://amzn.to/3cPCEMs), [AliExpress](https://s.click.aliexpress.com/e/_Dm43n6J)) or SD2SP2 ([Amazon](https://amzn.to/3I1cCSl), [AliExpress](https://amzn.to/3PNamBe))
* FAT32 or exFAT formatted SD card

Links above are affiliate and I get small comission 💵 if you buy these products. Thanks to everyone who used links above 🙏

## 2. Flashing Raspberry Pi Pico board

Go to [the latest release page](https://github.com/webhdx/PicoBoot/releases/latest) and download `picoboot.uf2` file. Now connect Raspberry Pi Pico board to your computer while holding `BOOTSEL` button pressed. If it's been done correctly you'll see `RPI-RP2` mass storage device show up. Drag and drop `picoboot.uf2` file to that device. It'll automatically eject and green LED will light up if it was programmed correctly. Unplug USB cable from Pico and proceed with hardware installation.

## 3. Preparing SD card

Format your SD card to FAT32 or exFAT. Download the latest Swiss release from [here](https://github.com/emukidid/swiss-gc/releases/latest) and grab `swiss_rXXXX.dol` file, rename it to `ipl.dol` and copy to the root of your SD card.

## 4. Hardware installation

![Wiring diagram](https://raw.githubusercontent.com/webhdx/PicoBoot/main/assets/Wiring%20diagram.jpg)

❗ Wire length and diameter plays a huge role! Keep the wires as short as possible, 10 cm (~4 inches) is a sweet spot. Anything longer can result in no video issue and don't work reliably. Use high quality 28 AWG cables for data lines and 26 AWG for 3.3V and GND.