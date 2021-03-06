# FarmBot 2020 Repo

# Farmbot

## Original FarmBot GitLab repo.
https://gitlab.op-bit.nz/BIT/Project/FarmBot/FarmbotWiki


### 3D files
https://sketchfab.com/farmbot/models
</br>
https://www.thingiverse.com/thing:2372024
</br>
Follow the link to find all the necessary 3D files for FarmBot. This can but used on a 3D print, CNC and lazer cutter.

### FarmBot set up
https://software.farm.bot/docs/configurator
</br>
https://software.farm.bot/docs/farmbot-os
</br>
</br>
Important info for server access:</br>
https://software.farm.bot/docs/for-it-security-professionals

### FARMBOT SETUP – Print Out

1)	Flash a fresh Farmbot OS onto the SD Card
2)	Insert SD Card into Farmbot Device
3)	Power on Farmbot Device
4)	On your mobile/laptop device go to Wi-Fi and select Farmbot
5)	Go to your browser and enter 192.168.24.1
6)	Select Wi-Fi option
7)	Click on manual input and enter “OP-Mobile”
8)	Use the key “bpdyHDPnBjWR”
9)	Enter your Farmbot account
10)	Farmbot will now deactivate its own Wi-Fi and connect to OP-Mobile
11)	Connect to “eduroam” on your mobile/laptop device
12)	Open a browser and go to “my.farm.bot”
13)	Wait for it to sync
14)	Go to device tab and select the Arduino/RAMPS firmware
15)	Wait for it to install may take a minute or two
16)	You’re a goat




### Members
Anthony
</br>
Damian
</br>
Woody

### Todo:
 - Limit/bump switches
 - Wire up tool heads
 - Automate paths and operation

### Done:
 - The Team tightened up Farmbot and made sure nothing was loose, we then connected farmbot up to a mobile network to make sure 
all the parts worked. after fiddling around with the farmbot interface, we go it to move.
 - 3d printing of weather resistant parts 99 percent complete.

# CNC Machines

## Set up
 - Open the folder containing the driver and the GRBL software.
 - Install the driver first then the software.
 - Install a third software for choice i.e. Scan2Cad (for converting images to the .nc file type that GRBL uses)
 - Use the third party software to creat the needed .nc file type for the machines.
 - Vectorizes and save the file you have just created.
 - Open the GRBL software and then open the .nc file you have created (this should bring up the image you just saved and have a  scrollable list of gcode line below which the machines will use to naviagte)
 - plug and power on machine of choice.
 - connect the machine via USB cable to the computer.
 - In the GRBL software the the machine should automatically connect and the 'send, pause and abort' buttons should be available.
 - If GRBL software dosnt connect open device manager(windows) and find the com port the usb is conneted to. 
 - Then go into GRBL, click Service, then settings, the connection and type in the correct port. 
 - Use the above buttons to control the machine.
 
 ### Lazer cutter specific
  WARNING:::WEAR LAZER GLASSES:::WARNING
 - create a file in InkScape, and follow this tutorial to generate the Gcode https://winder.github.io/ugs_website/
 - https://www.ctoom.com/tutorial/how-to-create-g-code-file-with-inkscape/
 - Once the gcode is generated,
 - move onto thehardware computer and import the gcode file into the unerversalGcodeSender java app
 - lazer cutter should be connected, if not restart computer(This is for issues with com port)
 - Use the on screen controls to move the cutter to a home point and set home.
 - click send to start gcode script.
 
 - ### Current bugs
 - gcode is not telling lazer to tun off inbetween lines, and drags its self to the next position.
