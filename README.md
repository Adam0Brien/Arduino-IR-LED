# Arduino-IR-LED
Code for my first working IR Remote. Turns on and off an LED when you press the power button

Equipment :
Breadboard
5 Wires 
IR Reciever + Remote
220 OHM resistor
LED (any colour)


Steps:

1 - put the ir reciever in the breadboard and set the R pin to 5v
then set the G to GND on the arduino
then set Y to any digital pin, In this case pin 7


2 - Set up a simple led ciruit using a 220 OHM resistor 
pin 13 (in this case) should only connect to the resistor and not the led

have the resistor go to another pin far away (out of connection) and have the Anode of the LED (long leg) connect to the resistor
and have the cathode (short leg) connect to the GND on the arduino.


Once this is all set up run the code and the light should turn on when the power button is pressed.


if not your remote might not be set to the reciever in this case use this link and find out the hex code for your power button and replace that in ```if (results.value == 0xFFA25D) ```
