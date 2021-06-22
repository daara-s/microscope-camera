# microscope-camera

## Goal
Develop an affordable computer with a camera for 4 microscopes:
* Leitz Fluorvert FU
* Leitz Aristoplan
* Leica DMIRB
* Olympus Stereo

Ideal scenario: Wi-Fi-enabled high speed image collection and cloud sync
#### Options:
* 2 HDMI outputs
* SSD image storage
* Ease of interaction

## Solutions
There are multiple ways to tackle the problem, from focusing on ease of use, 
affordability, to mondularity and programmability.
This project exploration will start with required materials.

### Mounting
The most common means of mounting a camera are via a trinocular head (phototube/photoport) or on an eyepiece tube.
C mounts are the most used adapters for camera attachment.

"A 'c-mount' is a 25.4mm (1 inch) threaded hole on the face of a camera. The c-mount adapter has a corresponding male-c-mount thread at one end.  At the microscope end the c-mount adapter terminates either in a mount that is highly specific to each model of microscope (there is no universal mount), this is the most common type.  Or the c-mount adapter is designed to replace an eyepiece and will fit into a 23.2mm internal diameter eyepiece tube or phototube port, a further adapter allows this type of adapter to fit a 30, 30.5 or 31.75mm internal diameter eyepiece tube."
[Source](https://www.gtvision.co.uk/epages/es141397.sf/en_GB/?ObjectPath=/Shops/es141397/Categories/Microscope_Accessories/Microscope_Parts/Microscope_Camera_Adapters/CMount_Camera_Adapters)

Solution: **Use an eyepiece tube C mount adapter** 

Note: will need to confirm eyepiece tube dimensions with calipers in case multiple adapters are required (data not in manuals)

### Camera
3 options:
* DSLR camera
  * requires DSLR mount adapter
* off the shelf microscope camera
  * simplest to use
  * expensive
  * requires SD card + monitor, or computer/laptop for USB
* RPi HD camera
  * cheapest
  * requires Raspberry Pi computer
  * programmable, modifiable
  * requires set-up and coding
  * functions can be automated
