# Demonstration Project for Microchip AVR MCUs

The repository contains 2 projects: 
1. OLED_DISPLAY_4CHAR: 
	Watch or counter with 4 digits representing seconds and minutes. The Display displays 4 digits plus a colon in Indie Flower Font, size 40 pixels. The counter starts immediately atfer boot and increases seconds. 
2. OLED_DISPLAY_6CHAR: 
	Watch with 6 digits plus 2 colons, representing a watch with hours, minutes, seconds. 
	
# Used Software
The source code is a demonstration of displaying huge characters in any kind of Font. The fonts have been created with the python code in https://github.com/jdmorise/TTF2BMH. The description is still WIP
Several Fonts can be downloaded from https://github.com/jdmorise/AVR_BMH-fonts. 

# 
The code contains the following functions and libraries: 
main.c - main project, the timer, and the interrupt routines
i2c.c/i2c.h - I2C abstraction layer
lcd.c/lcd.h - definitions and functions to control the OLED display
fonts - folder containing all relevant fonts

