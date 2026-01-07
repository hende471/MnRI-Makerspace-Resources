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


## Create a Gcode File

Import your part's STL file into the Slicing software. For the TAZ6 and the Ultimaker printer, you need to use the Cura slicing software. If you're using the MNRI computer, in a new terminal type the following command:

```bash
./cura_lulzbot.AppImage # For the TAZ6
./cura_ultimaker.AppImage # For the Ultimaker
```

To import your part in Cura, click the folder icon on the left. Now you can select your part. Once you have imported the part, first ensure that the orientation of the part is correct. You can add multiple parts to the print bed as well. 

The TAZ6 traditionally uses 2.85 mm filament however you can use the standard 1.75 ~ 1.8 mm filament as well. In the Slicing software make sure that the Profile is set accordingly (select high detail 1.8 mm if you're using 1.75 mm filament). 

Depending on your part, you may need to add supports. Click the support check box especially if there are overhanging pieces in your part. You can also choose the infill percentage. The infill percentage determines how much filament is used as a percentage of the total volume of the part. 100% infill means that 100% of the volume will be printed. For larger parts you could use lower infill percentages between 20/40. For load bearing parts, use higher infill between 60/100.

Lastly when printing multiple parts, make sure that there is adequate space between parts particularly if you are using a "brim" on each part. Brims are useful as they help with bed adhesion. If your first layer seems to not stick too well and warp, using a brim may cause the issue to go away. 

## Schedule Time With The Printer


## Configure Printer


## Print Part


## Clean Up
