# "Color PIN Diagram" for Bigtreetech Octopus V1.0 and Octopus V1.1 Board:

This repository contains JPG and PDF files for the BIGTREETECH's Octopus V1.1 board.

## The PDF file of the "Color PIN Diagram" for the Octopus V1.0 and Octopus V1.1 Board:

### Why use the PDF file of the "Color PIN Diagram":

The PDF file looks the same as the JPG file. You can enlarge the image for both file types to get all the details, but the PDF file contains URL links that will take you to websites that contain further information.  For example there are URL links that will take you to the processor data sheet.  If the color diagram contains a URL in text then just click on the URL and the PDF will take you to that URL.

You can view the PDF in your browser by clicking on the filename ["BIGTREETECH-Octopus-V1.1-color-PIN.pdf"](https://github.com/GadgetAngel/BTT_Octopus_Color_PIN_Diagram/blob/main/BTT_Octopus_V1.1_Color_PIN_Diagram/BIGTREETECH-Octopus-V1.1-color-PIN.pdf) and then hit the download button.

## A Picture of the "Color PIN Diagram" for the Octopus V1.0 and Octopus V1.1 Board:

You can download the JPG file for this "Color PIN Diagram" by clicking on the file ["BIGTREETECH-Octopus-V1.1-color-PIN.jpg"](https://github.com/GadgetAngel/BTT_Octopus_Color_PIN_Diagram/blob/main/BTT_Octopus_V1.1_Color_PIN_Diagram/BIGTREETECH-Octopus-V1.1-color-PIN.jpg) and then hit the download button.  Again, to download the PDF just click on the filename ["BIGTREETECH-Octopus-V1.1-color-PIN.pdf"](https://github.com/GadgetAngel/BTT_Octopus_Color_PIN_Diagram/blob/main/BTT_Octopus_V1.1_Color_PIN_Diagram/BIGTREETECH-Octopus-V1.1-color-PIN.pdf) and hit the download button.

![JPG of Color PIN Diagram](BIGTREETECH-Octopus-V1.1-color-PIN.jpg)

## Picture of the Original PIN Diagram from Bigtreetech for the Octopus V1.0 and Octopus V1.1 Board:

![JPG of original PIN Diagram](images/BIGTREETECH-Octopus-V1.1-original-PIN.jpg)

## The Original Bigtreetech Wiring Diagram for the Octopus V1.0 and Octopus V1.1 Board:

### For general purposes:

![Original Wiring Diagram](images/BIQU-Octopus-wiring-diagram-V1.0-2021-7-9.png)

## For Voron 2.4 builders:

You can find Bigtreetech's Voron 2.4 wiring diagram at https://github.com/bigtreetech/BIGTREETECH-OCTOPUS-V1.0/blob/master/Octopus%20works%20on%20Voron%20v2.4/Firmware/BTT_OctoPus_Voron2.4_Wiring_English.pdf

## Bigtreetech has a GitHub repository for the Octopus V1.0 and Octopus V1.1 Board:

The Bigtreetech GitHub repository is located at https://github.com/bigtreetech/BIGTREETECH-OCTOPUS-V1.0

## Klipper firmware supports the Octopus V1.0 and Octopus V1.1 Board:

Here is the link to the config file on GitHub for the Octopus V1.1 board https://github.com/Klipper3d/klipper/blob/master/config/generic-bigtreetech-octopus.cfg.

Here is the link to the Klipper configuration file for the Voron 2.4 printer on the Voron 2.4 GitHub site https://github.com/VoronDesign/Voron-2/blob/Voron2.4/firmware/klipper_configurations/Octopus/Voron2_Octopus_Config.cfg

Since the PB7 PIN is shared between the PROBE connector and the BLTouch header you will only be able to use one of these two connectors.

If you decide later you want to look for a free I/O pin please do not make the mistake and think that if you use the PROBE connector for the proximity sensor then you have a free I/O pin on the BLTouch header.  That is NOT the case since PB7 is tied to both connectors.

If you are using the "PROBE" connector for a proximity sensor you will need to add a [probe] section to the "generic-bigtreetech-octopus.cfg" file and ensure that the sensor_pin: PB7

Please use the "Color PIN Diagram" in this repository to obtain the correct PIN assignments.

If you decide to flash a new bootloader to the Octopus V1.1 board (you should not need to because you can upload the new Klipper firmware using the micro-SD card reader) and find that the micro-SD card bootloader no longer works you will want to return the board to its shipment state by finding the original bootloader and "bootloader+firmware" files at https://github.com/GadgetAngel/BTT_SKR_13_14_14T_SD-DFU-Bootloader/tree/main/bootloader_bin/backed_up_original_bootloaders

