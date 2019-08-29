# Demonstration Project for Microchip AVR MCUs showing big, arbitrary fonts on an SSD1306 128 x 64 OLED display

The repository contains 2 projects: 
1. OLED_DISPLAY_4CHAR: 
	Watch or counter with 4 digits representing seconds and minutes. The Display displays 4 digits plus a colon in Indie Flower Font, size 40 pixels. The counter starts immediately atfer boot and increases seconds. 
2. OLED_DISPLAY_6CHAR: 
	Watch with 6 digits plus 2 colons, representing a watch with hours, minutes, seconds. 
	
# Used Software
The source code is a demonstration of displaying huge characters in any kind of Font. The fonts have been created with the python code in https://github.com/jdmorise/TTF2BMH. The description is still WIP
Several Fonts can be downloaded from https://github.com/jdmorise/AVR_BMH-fonts. 

# Code Overview
The code contains the following functions and libraries: 
main.c - main project, the timer, and the interrupt routines
i2c.c/i2c.h - I2C abstraction layer (using the hardware TWI block)
lcd.c/lcd.h - definitions and functions to control the OLED display
fonts - folder containing all relevant fonts, including Indie Flower in different sizes and a generic 6x8 ascii font

# Contributors
The LCD  library has been developed by Michael Köhler, it was adapted and split into two parts to separate the LCD and I2C libraries. The basic description is found in a microcontroller.net forum. 
https://www.mikrocontroller.net/topic/415651
The zip file containing the library has been uploaded to this repo in the archive folder. 
