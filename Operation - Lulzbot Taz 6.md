# Operating Documentation for the Lulzbot Taz 6

## Overview

Using the printer involves several steps. Here is a summary of the steps
- Create a Finished 3D Model
- Create a Gcode File
- Schedule Time With The Printer
- Configure Printer
- Print Part
- Clean Up

## Create a Finished 3D Model

The first step is to export your 3D model to the STL format. STL (Stereolithography) is a standard file type for 3D printing that most CAD software packages use. It is also the most compatible file type for the Slicing software relevant in the next section. If you want to use the machine in the makerspace, make sure to save the STL in a USB drive. 


## Create a G-code File

Import your part's STL file into the Slicing software. For the TAZ6 and the Ultimaker printer, you need to use the Cura slicing software. If you're using the MNRI computer, in a new terminal type the following command:

```bash
./cura_lulzbot.AppImage # For the TAZ6
./cura_ultimaker.AppImage # For the Ultimaker
```

To import your part in Cura, click the folder icon on the left. Now you can select your part. Once you have imported the part, please make sure that the orientation of the part is correct. You can add multiple parts to the print bed as well. 

The TAZ6 traditionally uses 2.85 mm filament; however, you can also use the standard 1.75 mm to 1.8 mm filament. In the slicing software, make sure that the Profile is set accordingly (select high detail 1.8 mm if you're using 1.75 mm filament). 

Depending on your part, you may need to add supports. Click the support check box, especially if there are overhanging pieces in your part. You can also choose the infill percentage. The infill percentage determines how much filament is used as a percentage of the total volume of the part. 100% infill means that 100% of the volume will be printed. For larger parts, you could use lower infill percentages between 20/40. For load-bearing parts, use a higher infill between 60/100.

Lastly, when printing multiple parts, make sure that there is adequate space between parts particularly if you are using a "brim" on each part. Brims are useful as they help with bed adhesion. If your first layer seems to not stick too well and warp, using a brim may cause the issue to go away. 

### Exporting G-code

Once you have the print settings dialed in, you can export the G-code to an SD card. To print on the 3D printers in the MNRI makerspace, we use SD cards to upload the gcode onto the printer. Simply add your SD card to the host machine (wherever you have your slicer software), select the option to export gcode, and make sure to export it to the SD card. Now you can eject the SD card, which should have the gcode uploaded. 

> Note: the above 3 steps can be done on any machine. You will need to install the [CURA slicer](https://curaslicer.com/) software.

## Schedule Time With The Printer


## Configure Printer
If you are using the TAZ6, most of the configuration is done on the slicing software. The TAZ6 uses a borosilicate plate as the base on which your part will be printed. Materials like PetG, or high infill PLA, you may notice that the part is stuck to the borosilicate plate. Typically, you would use a hammer and a screwdriver to dislodge the part; this may damage the plate. To avoid this, we recommend adding a layer of masking tape to the print bed, completely covering the print surface. This way, when you are done with your print, you can simply peel off the tape along with your part. 


## Print Part

To print the part, turn on the printer, and insert the SD card into the slot. Now you can select the print from SD option. Select your part and start the print. The printer will tell you how long the part is going to take to print. We recommend waiting for at least the first layer to print before walking away. This may take a few minutes as the Extruder and the print bed need to come up to temperature. 

## Clean Up
