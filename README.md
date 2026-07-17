# TP-LINK TL-WDR7400 language file
This repo is dedicated to this only JavaScript file contain all strings ( in Chinese ) used for the WebGUI.

**NOTE: plugin translations are not included in this file, requiring modification on the actual .htm file for each plugin.**

## Overview

The file contain about 1,500 lines (1,492), which only about ~1,300 lines are text strings, others are JS code.

can be found in: the ``` www/web-static/language ``` directory when extract base .bin file from SPI chip.

<img width="800" alt="image" src="https://github.com/user-attachments/assets/e69232fa-7d1a-417b-a908-e81f22152e7d" />

**To extract the .bin file, please use Binwalk, unsquashfs-tools, jefferson, sasquatch-Universal-Builder and install required dependencies. For installation, please refers to guides on those repo.**

## How to pull language file
  Before doing the extraction, please ensure that you have all the mentioned above dependencies installed correctly.
  (To WSL users, please run ```cd ~``` as some .symlink might be broken if extracted in the ```mnt/c``` )

  1. Get the base file from TP-LINK website: ( should be firmware.zip)
     ( In case no source or it's CN TP-link, use the raw binary taken from the SPI chip )
     
  2. Open terminal ( linux ) or CMD/PS then type "WSL" (Window)

  3. Check .bin file 
  ```
binwalk your_firmware.bin
  ```
  if ok, then extract file
  ```
binwalk -e your_firmware.bin
  ```
Which should make a new folder.

  4. Now, move to the ```language``` dir by using cd command, or ``` explorer.exe . ``` for WSL.
    ( for WSL, keep the dot to open file explorer at the current directory ).

      Keep in mind that, the ```www``` folder contains the neccessaries for WebGUI.
      the ```www``` in the jffs folder contains the .htm for interacting with plugins.
     
  6. Pull the file to your desired location. Now you have done the work, take a rest~!
## How to apply
  By the time i write this, i have just gotten the lang file from the firmware. i might take a while for me to figure it out. Please make a discussion for any tips u guys can give me pls, and thx for reading this README.md

## Credits

 thanks my brother for helping me making the sasquatch works on my PC  ToT.
