# bpim2z-ov5640
Hi, you are looking at the configuration of an image with a working OV5640 camera sensor including auto focus!

The DTS-Files have to be copied to arch/arm/boot/dts/ and the ov5640.c file replaces the one at drivers/media/i2c/.

Alternatively, you can apply the patch in this repo which combines all changes.

I uploaded a freshly built [image](https://github.com/treim-de/bpim2z-ov5640/releases/tag/latest) with the following specs:
- Kernel 5.10.89
- Debian 11 (Buster)
- XFCE desktop
- Changed Device Tree for OV5640 support
- Changed Driver for Auto-Focus support

Note that there are no hardware changes necessary to enable AutoFocus (unlike some Youtube videos suggest)!

Please read [this section](https://github.com/Qengineering/BananaPi-M2-Zero-OV5640#ov5640) to learn how to get started and which camera to use.

# Thanks to:
- **Q-engineering** for creating [this image](https://github.com/Qengineering/BananaPi-M2-Zero-OV5640)
- **Wim van ‘t Hoog** for building [the device tree](https://wvthoog.nl/nanopi-ov5640-camera/) 
- **Rob Gries** for [this gist](https://gist.github.com/RobGries/b7beb724574f6da2ff660604980f6311)
- [This article](https://titanwolf.org/Network/Articles/Article?AID=ebcdfabe-a530-4192-af40-58a8eab0a8fa) on TitanWolf
