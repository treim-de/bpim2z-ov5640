# BPI M2 Zero with auto-focussing OV5640!
Hi, you are looking at the configuration of an image with a working OV5640 camera sensor including auto focus for the Banana Pi M2 Zero!

The DTS-Files have to be copied to arch/arm/boot/dts/ and the ov5640.c file replaces the one at drivers/media/i2c/.

Alternatively, you can apply the patch in this repo which combines all changes.

If you are like me and trust random strangers on the internet, I uploaded a freshly built [image](https://github.com/treim-de/bpim2z-ov5640/releases/tag/latest) with the following specs:
- Kernel 5.10.89
- Debian 11 (Bullseye)
- XFCE desktop
- Changed Device Tree for OV5640 support
- Changed Driver for Auto-Focus support

Note that there are no hardware changes necessary to enable auto focus on the BPI (unlike some Youtube videos suggest)!

Please read [this section](https://github.com/Qengineering/BananaPi-M2-Zero-OV5640#ov5640) to learn how to get started and which camera to use.

# Thanks to:
- **Q-engineering** for creating [this image](https://github.com/Qengineering/BananaPi-M2-Zero-OV5640)
- **Wim van ‘t Hoog** for building [the device tree](https://wvthoog.nl/nanopi-ov5640-camera/) 
- **Rob Gries** for [this gist](https://gist.github.com/RobGries/b7beb724574f6da2ff660604980f6311)
- [This article](https://titanwolf.org/Network/Articles/Article?AID=ebcdfabe-a530-4192-af40-58a8eab0a8fa) on TitanWolf

# Disclaimer
The driver took me hours to adapt from various sources on the internet and it works well for my use cases, but I have no experience building drivers (which is probably why it took so long) nor do I regularly compile kernels. Usage is **at your own risk!**

If you have any doubts about this image or this driver feel free to adapt it to your needs and build your own images :) 
If you make improvements please do notify me as I happily apply them.
