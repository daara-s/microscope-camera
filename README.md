# microscope-camera

## Goal
[Develop an affordable computer with a camera for 4 microscopes:](https://www.opencell.bio/summerprojects)
* [Leitz Fluorvert FU](https://www.opencell.bio/equipment/fluovert-fu-microscope)
* [Leitz Aristoplan](https://www.opencell.bio/equipment/leitz-aristoplan-microscope)
* [Leica DM IRB](https://www.opencell.bio/equipment/inverted-microscope)
* [Olympus Stereo](https://www.opencell.bio/equipment/sz40-olympus-microscope)

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

**Solution:** Use an eyepiece tube C mount adapter

Note: will need to confirm eyepiece tube dimensions with calipers in case multiple adapters are required (data not in manuals)

### Camera
3 options:
* DSLR camera
  * requires DSLR mount adapter
  * highest quality images
* off-the-shelf microscope camera
  * simplest to use
  * expensive
  * requires SD card + monitor, or computer/laptop for USB
* RPi HD camera
  * cheapest
  * requires Raspberry Pi computer
  * programmable, modifiable
  * requires set-up and coding
  * functionality can be automated

**Solution:** use RPi HD camera if cost/automation/programmability are a priority, else use off-the-shelf microscope camera

### Computer
If using a DSLR or off-the-shelf camera, images/videos can be saved onto an SD card, or via a computer/laptop over USB.
If using the RPi HD camera, a Raspberry Pi is recommended:
* RPi Zero for low cost
  * run as a headless server, allowing for control and image retrieval via a python webapp
* RPi 4 for performance
  * output to multiple HDMI monitors
  * run as a headless server
  * interfaced via touchscreen

**Solution:** dependent on camera choice and requirements

## Cost
Simplified cost breakdown for most affordable option:
* C mount adapter [£27](https://www.amazon.co.uk/Oumij-C-mount-Adapter-Microscope-Eyepiece-default/dp/B07XSCXDSQ/ref=sr_1_3?dchild=1&keywords=microscope+c+mount+adapter&qid=1624371122&sr=8-3)
  * assuming it fits all 4 microscopes
  * cost is variable based on material choice, quality, magnification, eyepiece diameter
* RPi HD camera [£50](https://thepihut.com/products/raspberry-pi-high-quality-camera-module)
  * may need lens attachment (further research required)
  * cable adapter may also be needed depending on which RPi it connects to
* RPi Zero [£10](https://thepihut.com/products/raspberry-pi-zero-w)
  * £34 for RPi 4 2GB

**Total:** £87 excluding cables, power supply, enclosure, extra adapters
