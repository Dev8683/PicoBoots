### Can I use new Pico W board?

It depends. According to the reports it works but the green LED won't light up which may be confusing at first. I haven't tested it personally therfore I can't provide you with any support at this time. It's planned to fully support Pico W and WiFi functionalities in the future.

### My console doesn't start - I see a black screen.

This indicates problem with wiring. Make sure there are no unintentional shorts near RTC-DOL (U10) IC. It's recommended to use wires as short as possible. The wires can't be too thin, you need at least 26 AWG for 3.3V and GND. Optimal location for PicoBoot is between controller port board and fan assembly. Especially I do not recommend installing PicoBoot in Serial Port 1 slot - it makes wire runs too long and may stop working with future updates! Use only official diagrams, any alternative soldering points and chip locations are not guaranteed to work.

### I don't understand how it's better than XenoGC

XenoGC is a drive modchip, it can only patch disc data on the fly. This means you have to use a boot disk to run Swiss and play games from an SD card. PicoBoot uses completely different approach - injects custom payload during console boot sequence. This means it can load any application instead of a built in GameCube menu. It will work even if your disc drive is not working.

### I installed your modchip and now my console doesn't work

Sorry. I do not take reponsibility for any damage done by installing this modchip. Do it at your own risk!

### Can I use other RP2040 boards?

Yes, go for it. Just respect the [license agreements](LICENSE) and don't expect me to provide any support for your board. PicoBoot only supports official Raspberry Pi Pico module at the moment.

### Will it work if I have XenoGC installed?

Yes, you can use it with XenoGC intalled.

### I appreciate your work. Can I support you in any way?

This project is free and available for everyone. If you want to support it anyway, consider using [:heart: Sponsor](https://github.com/sponsors/webhdx) button.