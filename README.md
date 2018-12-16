# PiBatteryGague
It is a battery gague integrated charging function.
Becareful of the position. Pi Battery Gague must be connected with Pin(3~8).
Any size of 3.7V Li-battery is OK, it could also work as a small UPS.
![](https://github.com/lspoplove/D-duino/blob/master/Documents/pibatterygague.jpg)

## Installation
1.Open the I2C interface of the Raspberry Pi.If it is already open, skip this step. Open Terminal, type the following command, and press Enter:
```
 pi@raspberrypi:~ $ sudo raspi-config
 ```
Then use the up and down keys to select “5 Interfacing Options” -> “P5 I2C” and press Enter to confirm “YES”. Reboot the Raspberry Pi.  
2.Installing Python libraries and git (networking required). If it is already installed, skip this step. In the Terminal, type the following commands, and press Enter:  
```
pi@raspberrypi:~ $ sudo apt-get update
pi@raspberrypi:~ $ sudo apt-get install build-essential python-dev python-smbus git
```
3.Download the driver library and run it. In Terminal, type the following commands, and press Enter:
```
pi@raspberrypi:~ $ git clone https://github.com/DFRobot/DFRobot_MAX17043.git
pi@raspberrypi:~ $ cd ~/DFRobot_MAX17043/RaspberryPi/python
pi@raspberrypi:~/DFRobot_MAX17043/RaspberryPi/python $ python DFRobot_MAX17043.py
```
## Read Battery Voltage, Remaining Power and Set Low Power Interrupt Alert
```
pi@raspberrypi:~/DFRobot_MAX17043/RaspberryPi/python $ cd readAndInt
pi@raspberrypi:~/DFRobot_MAX17043/RaspbeeryPi/python/readAndInt $ python readAndInt.py
```
## Results
