# MKS_ROBIN_E3D_2.1.2.1
Configuration and BIN file for MKS Robin E3D for:
- Ender 3.
- BMG (Dual gear with reduction) Extruder.
- TMC2209 stepper drivers.
- Steps setted to: 80 80 400 404.2 

You can also test by changing the steps/mm in the configuration menu directly in the printer, until you get the desired calibration.
*(Original steps configuration is: 80 80 400 93)*

Based on Marlin 2.1.2.1

# Especial settings

- Change filament
- Load filament
- Unload filament
- Save settings (Saves to SD Card)
- Custom speeds for load and unload filament
- Changed acceleration control to suit Ender 3 mechanics and avoid damage

# Instructions

Download the latest version of:

1. [Marlin Firmware](https://marlinfw.org/)

Install the following extensions in **VSCode**, or **VSCodium**

2. [ms-vscode.cpptools](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools)
3. [platformio.platformio-ide](https://marketplace.visualstudio.com/items?itemName=platformio.platformio-ide)
4. [MarlinFirmware.auto-build](https://marketplace.visualstudio.com/items?itemName=MarlinFirmware.auto-build)

Once installed, go to the left panel of VSCode and clic over the PlatformIO icon.

Go to Quick Access -> Updates -> Platform updates

Update all items available for update

Use the Configuration.h and Configuration_adv.h as templates for your configuration. Try to use Meld (Linux) or WinMerge (Windows) for file comparision between your current configuration files and the ones provided here to make it easier to check the changes, this is optional though.

**Be careful!**
Verify the bed dimensions, temperatures and drivers used, otherwise you could damage your printer. 
The first thing to do after flashing is to turn off and then turn on the printer.
Calibrate the steps/mm to check if the ones specified here (202.1 for Extruder) are correct, otherwise you would need to modify that value.
Run the autohome instruction from the printer, be ready to turn off the printer in case of crazy speeds or wrong direction!!

The included Robin_e3d.bin file, is a ready to flash file, just put it in your SD Card, insert the
SD card in the board, and power on. The flash process will start automatically. 
