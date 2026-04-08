# Mara X Shot Timer
An arduino based shot timer for the Lelit Mara X prosumer espressor machine. 

## Existing projects

1. https://github.com/SaibotFlow/marax-monitor (The pictures about the wiring are very helpful)
1. https://github.com/DiSanzes/Mara-X2-ShotTimer (forked the first)
1. https://github.com/snafuz/MaraXDisplay (forked the second)
      
## Objective 1

The project runs on most Arduino boards or ATmega chips. 

Reasoning: Most existing projects use ESP32 or better with WiFi capabilities which none of the projects need nor use. ATmegas that support two serial I/Os at the same time, get the job done. 

## Objective 2

The project uses, only when necessary, currently maintained dependencies. 

Reasoning: For the longest time, most of the listed projects were using a deprecated library. The aim is to handcode as much as possible to make the project run on smaller hardware as well. Without any dependencies will most likely not be possible since libraries for the display and the software serial are needed. 

## Compatibility

Adafruit SSD1306 for the display: https://github.com/adafruit/Adafruit_SSD1306  
Comptaible with most ATmega and ESP* but not ATtiny85.

# Materials

* Board
* Display
* Voltage regulator

# Power supply

## Pins

* 1 - VCC (12V)
* 2 - GND
* 3 - Receive (RX)
* 4 - Transmit (TX)

Note: I must make a huge mistage there. The 12V drops to 1.7V or less when connected with a buck converter, but before the converter. If anyone has a datasheet of the pins from the Mara X board, I'd be extremly thankful. 

## USB

## 9V block battery

### Switch

### Button

Power on
opener Transistor is letting energy flow
define output pin digital
after 120 000 seconds
signal 1 on output pin
power off

Circuit

https://forum.arduino.cc/t/vorstellung-und-erste-fragen-zur-selbstabschaltung-transistorschaltung/362576/16

## From Mara X with voltage regulator

### Circuit

https://www.circuits-diy.com/12v-to-9v-converter-circuit-using-lm7809-regulator-ic/

### Buy

https://www.ebay.de/itm/375340664282

