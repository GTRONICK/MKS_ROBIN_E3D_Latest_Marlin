# MKS_ROBIN_E3D_2.0.9.3
Configuration and BIN file for MKS Robin E3D for:
- Ender 3.
- BMG (Dual gear with reduction) Extruder.
- TMC2209 stepper drivers.
- Steps setted to: 80 80 400 404.3 

*(Original steps configuration is: 80 80 400 93)*

Based on Marlin 2.0.9.3.

# Especial settings

- Change filament
- Load filament
- Unload filament
- Save settings (Saves to SD Card)
- Custom speeds for load and unload filament

# Instructions

Download the latest version of:

1. Marlin firmware
2. PlatformIO extension for VSCode
3. Auto Build Marlin for VSCode

Once installed, go to the left panel of VSCode and clic over the PlatformIO icon.

Go to Quick Access -> Updates -> Platform updates

Update all items available for update

Use the Configuration.h and Configuration_adv.h as templates for your configuration. Try to use Meld (Linux) or WinMerge (Windows) for file comparision between you current configuration files and the ones provided here to make it easier to check the changes, this is optional tough.

**Be careful!**

Verify the bed dimensions, temperatures and drivers used, otherwise you could damage your printer. 
The included Robin_e3d.bin file, is a ready to flash file, just put it in your SD Card, insert the
SD card in the board, and power on. The flash process will start automatically. 
