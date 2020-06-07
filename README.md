# piLCD3

# Nexgen-Gadgets Raspberry Pi 3.5 Touchscreen LCD Drivers type-3

# How to install:
  
1.)Step1, Install Raspbian <br>
====================================================
  a)Download Raspbian official mirror:<br>
  https://www.raspberrypi.org/downloads/<br>
  b)Use “Balena Etcher” https://www.balena.io/etcher/ to burn the raspbian image into your TF Card<br>
     
2.) Step2, Clone this repository onto your pi and install<br>
====================================================
Use SSH to connect the Raspberry Pi, <br>
And Ensure that the Raspberry Pi is connected to the Internet before executing the following commands:
-----------------------------------------------------------------------------------------------------

```sudo rm -rf piLCD3```<br>
```git clone https://github.com/nexgen-gadgets/piLCD3.git```<br>
```chmod -R 755 piLCD3```<br>
```cd piLCD3/```<br>
```sudo ./LCD35a3-install```<br>

Raspberry Pi will then reboot and LCD will be working.

# How to rotate the display direction

This method only applies to the Raspberry Pi series of display screens, other display screens do not apply.

### Method 1, If the driver is not installed, execute the following command (Raspberry Pi needs to be connected to the Internet):

```sudo rm -rf piLCD3```<br>
```git clone https://github.com/nexgen-gadgets/piLCD3.git```<br>
```chmod -R 755 piLCD3```<br>
```cd piLCD3/```<br>
```sudo ./LCD35a3-install 90```<br>  <-- 90 means the display will rotate 90 degrees

After execution, the driver will be installed. The system will automatically restart, and the display screen will rotate 90 degrees to display and touch normally.<br>
(' 90 ' can be changed to 0, 90, 180 and 270, respectively representing rotation angles of 0 degrees, 90 degrees, 180 degrees, 270 degrees)<br>

### Method 2, If the driver is already installed, execute the following command:

```cd piLCD3/```<br>
```sudo ./LCD35a3-install 90```<br>

After execution, the system will automatically restart, and the display screen will rotate 90 degrees to display and touch normally.<br>
( ' 90 ' can be changed to 0, 90, 180 and 270, respectively representing rotation angles of 0 degrees, 90 degrees, 180 degrees, 270 degrees)<br>
(If the rotate.sh prompt cannot be found, use Method 1 to install the latest drivers)
