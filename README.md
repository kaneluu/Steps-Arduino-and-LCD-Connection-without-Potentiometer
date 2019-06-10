# Steps-Arduino-and-LCD-Connection-without-Potentiometer
I. Parts Needed:
_Hardware: Arduino UNO, 16x2 LCD, wires.
_Software: Arduino IDE.
II. 16x2 LCD Introduction:
_It has 16 pins and start from left to right they are:
	+VSS or GND pin is connected with the GND pin on the Arduino
	+VCC or VDD pin connects to the 5v pin on the Arduino 
	+NOTE: VSS and VDD are 2 power supply pins
	+Vo is the display contrast pin which controls how thick the character would be shown
	+RS is the register select pin and is used for selecting whether we will send commands (when we set it on low states or 0v) or data to the LCD (when we set it on high states or 5v)
	+RW pin selects the mode whether we read or write on LCD. Write is for writing or sending commands and read is used by the LCD itself.
	+E pin enables the writing to the text eight registers (or pins from D0-D7)
	+D0-D7 are data pins
	+A (anode) and K (cathode) are for the LCD backlights.
III. Arduino and LCD connection
_PIN1 or VSS to ground
_PIN2 or VDD or VCC to +5v power
_PIN3 or Vo to ground (gives maximum contrast best for a beginner)
_PIN4 or RS (Register Selection) to PIN0 of ARDUINO UNO
_PIN5 or RW (Read/Write) to ground (puts LCD in reading mode eases the communication for user)
_PIN6 or E (Enable) to PIN1 of ARDUINO UNO
Starting from connecting registers to the Arduino, it is your options to choose different pin numbers on the Arduino.
_PIN11 or D4 to PIN8 of ARDUINO UNO
_PIN12 or D5 to PIN9 of ARDUINO UNO
_PIN13 or D6 to PIN10 of ARDUINO UNO
_PIN14 or D7 to PIN11 of ARDUINO UNO
_PIN15 or A to 5v of ARDUINO UNO
_PIN16 or K to ground
IV. Writing Code on the Arduino IDE (In two other files)
