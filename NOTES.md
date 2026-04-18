# Notes

This file contains notes about my process and thoughts during the project. 

# Materials

* Board
* Display
* Voltage regulator

# Power supply

Initially I wanted the coffee machine to power the arduino board. That turned out to be more difficult than expected. 

Pins 3 and 4 of the Mara X board are used for the serial communication. Pin 2 seemed to be ground and pin 1 seemed to supply 12V current. But the current drops  (to about 1.7V) as soon as the tiniest load is applied. 

**Pins:**
* 1 - VCC (12V)
* 2 - GND
* 3 - Receive (RX)
* 4 - Transmit (TX)

My next idea was to user a 9V block battery or a 18650 cell with a button and a self-latching circuit that turns itself off when unused for some time. 

Here is an example:  
https://forum.arduino.cc/t/vorstellung-und-erste-fragen-zur-selbstabschaltung-transistorschaltung/362576/16

In practice, it wasn't a good solution. 

Lastly, I've attached the coffee machine, the coffe grinder, and USB-power supply for the ardunio board on the same extension cord with switch. I consider this topic closed. 



# Resources

* https://www.circuits-diy.com/12v-to-9v-converter-circuit-using-lm7809-regulator-ic/
* https://www.ebay.de/itm/375340664282
