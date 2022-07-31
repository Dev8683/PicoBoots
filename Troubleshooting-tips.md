## My console boots to vanilla GC menu

In most cases this suggests there are issues with your SD card setup. Many people experienced this with SD2SP2 adapters which are very often terrible quality. I suggest trying different SD2SP2 adapter, preferably sideloading one (so called "GB Player compatible") which are, in my experience, more reliable. Getting one of memory card form factor adapters (SD Gecko, WiiSD) is also a good idea. These adapters pretty much always work. Also this is the adapter you want to get if you are using DOL-101 model.

Starting with [PicoBoot v0.2](https://github.com/webhdx/PicoBoot/releases/tag/v0.2) release you can hold D-Pad Down during boot to see debug output from iplboot. If you see white text on black screen it means PicoBoot is installed correctly and your problem is caused by SD card setup.

[[/assets/iplboot_debug_output.png|IPLBoot debug screen]]

## The console is running but it doesn't display anything on the screen

This means PicoBoot probably injected the payload but it was malformed due to interference inducted on the wires. This happens when you've used inappropriate wires for the installation. There is a golden rule: use as short wires as possible. 10 centimeters (~4 inches) is what I'd consider as a maximum recommended length. Anything over that will not work reliably. The type of wire is also very important. Use 28 AWG for data lines and 26 AWG for 3.3V and GND. Don't use thick, inflexible wires because it's very easy to put too much stress on the soldering points and rip some pads or in worst case legs on U10 chips. If that happens it's a game over for your console and it's beyond fixable at that point.

## Power light comes off shortly after hitting the power button

This indicates shorted power line. Check your soldering and make sure wires are not touching any other point than the one mentioned in the diagram. Please be careful, there is 12V power line on the SP1 connector where you need to solder 3 wires. It's possible to short it to data lines and fry CPU.

