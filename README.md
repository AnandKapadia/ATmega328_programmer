AT Programming Shield
==========

##BOM
* Shield Board (eagle schematic provided)
* Arduino Uno
* Chip to Program, either an ATTiny85, ATmega328P-PU, ATmega328P(TQFP)
* 16Mhz Crystal
* Capacitors for Crytsal (22 pF) x2
* 10uF Cap 
* 10k Resistor (0603)
* 330 Resistor (0603)
* 4 Slide Switches
* SMD LED (1206)
For a detailed list please see the BOM

##Here is what the shield looks like. 

![alt text](https://github.com/AnandKapadia/ATmega328_programmer/blob/master/images/cad_1.png "CAD 1")

![alt text](https://github.com/AnandKapadia/ATmega328_programmer/blob/master/images/cad_2.png "CAD 2")

![alt text](https://github.com/AnandKapadia/ATmega328_programmer/blob/master/images/osh.png "OSH Park")

Image: 
![alt text]( "Image")

Soldered: 
![alt text]( "Soldered")

##How To Use
NOTE: You can only program one board at a time. 

From top to bottom, here is what each switch does. 
* Switch 1 (Connection to Pin 1 of ATMega): Arduino 10 <--> Arduino Reset
* Switch 2 (Connection to Pin 3 of ATMega): Disconnected <--> Arduino TX
* Switch 3 (Conenction to Pin 2 of ATMega): Disconnected <--> Arduino RX
* Switch 4 : Arduino Reset connected to Capacitor (10uF) <--> Disconnected

For ATtiny85: 
* Switches 1-3 : Does not matter
* Switch 4 : To the Left (Reset connected to Cap)

For Bootloader onto ATMega (both forms):
* Switch 1: To the left (Arduino 10)
* Switch 2/3: To the left (Disconnected)
* Switch 4: To the right (Disconnected)
    
For Programming onto ATMega (both forms):
* Switch 1: To the Right (Arduino Reset)
* Switch 2/3: To the Right (Rx/Tx)
* Switch 4: To the right (Disconnected)
* Note: Remove the arduino's built in mega chip to do this. 

