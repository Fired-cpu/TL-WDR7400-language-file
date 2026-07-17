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
        
