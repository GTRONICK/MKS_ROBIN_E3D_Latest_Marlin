# MKS_ROBIN_E3D_2.0.7.2
Configuration and BIN file for MKS Robin E3D, for Ender 3

Based on Marlin 2.0.7.2.

Download the latest version of:

1. Marlin firmware
2. PlatformIO extension for VSCode
3. Auto Buil Marlin

Once installed, go to the left panel of VSCode and clic over the PlatformIO icon.

Go to Quick Access -> Platforms

Update all items available for update

Use the Configuration.h and Configuration_adv.h as templates for your configuration. 

**Be careful!**

Verify the bed dimensions, temperatures and drivers used, otherwise you could damage your printer. 
The included Robin_e3d.bin file, is a ready to flash file, just put it in your SD Card, insert the
SD card in the board, and poweron. The flash process will start automatically. 
