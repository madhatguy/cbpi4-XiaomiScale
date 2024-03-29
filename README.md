# CBPi4 Xiaomi Scale

### This CBPi4 Plugin Contains A Sensor class of a Bluetooth Xiaomi scale and the logic of Fill step (filling a vessel with liquid)

### Installation:

You can install it directly via pypi.org:	
- sudo pip3 install cbpi4-XiaomiScale 

Alternatively you can install (or clone) it from the GIT Repo. In case of updates, you will find them here first:
- sudo pip3 install https://github.com/madhatguy/cbpi4-XiaomiScale/archive/main.zip

## Xiaomi Scale

### Setup

- Get your scale's mac address. You can get it via the "zepp life" app:
  - Download the app and connect your device as the device instructions show.
  - Once the device has been connected open the app and go to the profile tab.
  - You should see your device in the "My devices" section, tap it.
  - The value in the "Bluetooth address" field is your device's mac address.

*Works only on linux based systems

## Parameters:

- Configurable:
	- Xiaomi Scale device Mac address.
	- Offset (insert the base weight of the rig standing on the scale in KG).
	- Gravity (insert the gravity of the liquid you want to measure, in SG). This field is irrelevant if Display type is Weight.
	- Display Type. Choose whether you would like to see the sensor value as weight or as liquid volume.
	
- Fixed in Code:
	- Sensor sampling interval (maybe made configurable in future releases)

## Fill Step

## Parameters:

- Configurable:
	- Volume. The target volume to fill.
	- Actor. If none is given, this step only measures the volume.
	- Sensor - to measure to volume.
	- Reset - Choose whether you want to reset the sensor after this step is done.

Changelog:

- 28.01.23: (0.2.1) Added Toggle state (enable/disable sensor) action
- 06.09.22: (0.2.0) Initial release

### A Word of Caution

Please be careful using a Xiaomi Bluetooth scale, namely - do not put it in direct contact with hot things, and be careful to not shutter the glass.
I'm not responsible for whatever damage or injury that may happen as a result of your use of a Xiaomi Scale, or any other instrument.

### Credits

Thanks to lolouk44 for the code responsible for extracting the weight of the scale
