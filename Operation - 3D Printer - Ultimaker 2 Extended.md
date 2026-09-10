# Operating Documentation for the Ultimaker 2 Extended

<br>

## Overview

- [Create a Finished 3D Model](#create-a-finished-3d-model)
- [Create a G-code File](#create-a-g-code-file)
  - [Exporting G-code](#exporting-g-code)
- [Configure Printer](#configure-printer)
- [Schedule Time With The Printer](#schedule-time-with-the-printer)
- [Print Part](#print-part)
- [Clean Up](#clean-up)

<br>

## Create a Finished 3D Model

The first step is to export your 3D model to the STL format. STL (Stereolithography) is a standard file type for 3D printing that most CAD software packages use. It is also the most compatible file type for the slicing software relevant in the next section. If you want to use the machine in the makerspace, be sure to save the STL file to a USB drive.

<p align="center">
  <img src="./images/3d-Model.png" width="900" alt="3D model export">
  <br>
  <em>Make sure to export the part in the STL format.</em>
</p>

<br>
  
## Create a G-code File

Import your part's STL file into the slicing software. For the Ultimaker and the Ultimaker printer, you need to use the Cura slicing software. If you're using the MNRI computer, in a new terminal type the following command:

```bash
./cura_lulzbot.AppImage # For the Lulzbot
./cura_ultimaker.AppImage # For the Ultimaker
```

> **Note:** The following steps can be done on any machine. You will need to install the [CURA slicer](https://curaslicer.com/) software.

<p align="center">
  <img src="./images/slicer1-ultimaker.png" alt="CURA slicer interface">
  <br>
  <em>The CURA slicer application page. Here you will find all the necessary tools to create G-code for the Ultimaker printer.</em>
</p>

<br>

> **Interface Overview:**
> 1. Import your part from files (Not shown, but the icon is in the same place as in the other slicer)
> 2. Part placement settings
> 3. Select filament type (In the ultimaker slicer, you can adjust this in the materials tab)
> 4. Print and printer settings
> 5. Start slicing

 <br>

To import your part in Cura, click the folder icon on the left. Once you have imported the part, make sure that the orientation of the part is correct. You can add multiple parts to the print bed as well.

<p align="left">
  <img src="./images/slicer2-ultimaker.png" width="400" alt="Printer settings">
  <br>
  <em>The printer settings tab contains the different parameters that can be adjusted for the print job.</em>
</p>

Depending on your part, you may need to add supports. Click the support checkbox, especially if there are overhanging pieces in your part. You can also choose the infill percentage. The infill percentage determines how much filament is used as a percentage of the total volume of the part. 100% infill means that 100% of the volume will be printed. For larger parts, you could use lower infill percentages between 20-40%. For load-bearing parts, use a higher infill between 60-100%.

Lastly, when printing multiple parts, make sure that there is adequate space between parts, particularly if you are using a "brim" on each part. Brims are useful as they help with bed adhesion. If your first layer does not seem to stick well and warps, using a brim may resolve the issue.

### Exporting G-code

Once you have the print settings dialed in, you can export the G-code to an SD card. To print on the 3D printers in the MNRI makerspace, we use SD cards to upload the G-code onto the printer. Simply add your SD card to the host machine (wherever you have your slicer software), select the option to export G-code, and make sure to export it to the SD card. Now you can eject the SD card, which should have the G-code uploaded.

<p align="left">
  <img src="./images/slicer3-ultimaker.png" width="400" alt="G-code export">
  <br>
  <em>Make sure to export to the SD card volume once the G-code is ready.</em>
</p>

 <br>

## Configure Printer

If you are using the Ultimaker, most of the configuration is done in the slicing software. The Ultimaker uses a glass plate as the base on which your part will be printed. For materials like PETG or high infill PLA, you may notice that the part is stuck to the plate. Some might have learned to use a hammer and a screwdriver to dislodge the part; this may damage the plate. To avoid overly strong bed adhesion, we recommend adding a layer of masking tape to the print bed, completely covering the print surface. This way, when you are done with your print, you can simply peel off the tape along with your part.

 <br>

## Schedule Time With The Printer

To use this equipment, you must reserve time with it; the MnRI Makerspace is accessed by 200+ undergraduate students, graduate students, research staff, and faculty. Time reservation is part of what keeps the space orderly. 
 <br>
To reserve time with the printer, use [this Google form](https://docs.google.com/forms/d/e/1FAIpQLScbIme_WRaoYv4oweY1Eg8Ww8YcjrLJ1fDP2vGtmIavPTJHPw/viewform).

 <br>


## Print Part

To print the part, turn on the printer and insert the SD card into the slot. Select the print option.

<p align="left">
  <img src="./images/printer1-ultimaker.png" width="400" alt="SD card slot">
</p>

Unlike the Lulzbot, the ultimaker directly takes you to the SD card when you select the 'Print' option. 

<p align="left">
  <img src="./images/printer2-ultimaker.png" width="400" alt="Print from SD menu">
</p>

The printer will tell you how long the part is going to take to print. We recommend waiting for at least the first layer to print before walking away. This may take a few minutes as the extruder and the print bed need to come up to temperature.

<p align="left">
  <img src="./images/printer3-ultimaker.png" width="400" alt="Printer in operation">
</p>

 <br>

## Clean Up

Once your print is complete, follow these steps to properly clean up:

1. **Allow Cooling** - Wait for the print bed and extruder to cool down to a safe temperature before attempting to remove your part. This typically takes 5-10 minutes.

2. **Remove the Part** - If you used masking tape on the print bed, simply peel off the tape with the part attached. If printing directly on the borosilicate plate, use a flat scraper or putty knife to carefully separate the part from the bed. Work slowly to avoid damaging the print surface.

3. **Remove Support Material** - If your print included support structures, carefully remove them using pliers or wire cutters. Support material is designed to break away easily but may require some effort for intricate parts.

4. **Clean the Print Bed** - Remove any remaining masking tape, filament residue, or debris from the print bed. Wipe down the borosilicate plate with isopropyl alcohol if needed to ensure it's clean for the next user.

5. **Turn Off the Printer** - If no one else is scheduled to use the printer immediately after you, turn it off using the power switch.

6. **Clean Your Work Area** - Dispose of any scrap material, failed prints, or support structures in the appropriate waste bin. Leave the workspace clean for the next user.

7. **Post-Processing** (Optional) - Depending on your needs, you may want to sand, paint, or otherwise finish your part. This should be done away from the printer in a designated work area.
