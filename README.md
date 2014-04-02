Si7005
======

Library for communicationg with the Silabs Si7005 temperature/  humidity sensor over I2C.

For i2C connections to Sparkfun Pro Micro or Arduino Micro, physical wiring is as follows:

SDA connects to Arduino Micro pin Labeled 2 (not A2)
SCL connects to Arduino Micro, pin Labeled 3 (not A3)
GND connects to GND

POWER: i2C devices usually require power. Pins may be labeled VCC, 5V or 3V. (*** BE CAREFUL HERE ***) This may be connected to Arduino Micro under the following conditions. 
1) The i2C device consumes less current (ma) ,at all times, than your Arduino can provide.
2a) The i2C device consumes the same voltage that your Arduino provides.
2b) The i2C device consumes the less voltage that your Arduino provides, but has an added regulator that lowers the voltage to the correct level. Here's a trick: Place three 1N4007 diodes in series, to drop 5V down to 3V if you don't have a proper regulator on hand.


/*
 * ----------------------------------------------------------------------------
 * "THE BEER-WARE LICENSE" (Revision 42):
 * <jonas@jalling.dk> wrote this file.  As long as you retain this notice you
 * can do whatever you want with this stuff. If we meet some day, and you think
 * this stuff is worth it, you can buy me a beer in return.   Jonas Bo Jalling
 * ----------------------------------------------------------------------------
 */
#######################################
# Syntax Coloring Map For Si7005
#######################################

#######################################
# Datatypes (KEYWORD1)
#######################################

#######################################
# Methods and Functions (KEYWORD2)
#######################################

detectSensor	KEYWORD2
getTemperature	KEYWORD2
getHumidity	KEYWORD2
enableHeater	KEYWORD2
disableHeater	KEYWORD2
enableFastMeasurements	KEYWORD2
disableFastMeasurements	KEYWORD2


#######################################
# Instances (KEYWORD2)
#######################################

Si7005	KEYWORD2

#######################################
# Constants (LITERAL1)
#######################################




What ?
======
This is a Arduino library for the Silabs Si7005 temperature/humidity sensor.
The library makes it easy to use the sensor and all of its features.


Why ?
=====
Because I think it's an interesting sensor, and I wanted to test it. I couldn't find
any library or sample code on the internet, so i wrote my own.


Getting started
===============
Copy the directory Si7005 to you Arduino library folder.

Load the Arduino IDE and open the example program from the file menu.

The humidity measurement is dependant on the temperature measurement, and uses the last
measured temperature.
If no temperature measurement is done at all, a default value of 25.0C is used.


Who ?
=====
Written by Jonas Bo Jalling, <jonas@jalling.dk>


License ?
=========
/*
 * ----------------------------------------------------------------------------
 * "THE BEER-WARE LICENSE" (Revision 42):
 * <jonas@jalling.dk> wrote this file.  As long as you retain this notice you
 * can do whatever you want with this stuff. If we meet some day, and you think
 * this stuff is worth it, you can buy me a beer in return.   Jonas Bo Jalling
 * ----------------------------------------------------------------------------
 */
