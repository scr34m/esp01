#                                         ARDUINO UNO  WITH GPIO WORKING CONCEPT
# Components
                                Arduino UNO  
                                ESP8266 ESP-01 
                                Connecting Wires 
                                Bread Board or  DOT board
                                Push Button
#                                          Connecting the ESP8266 to an Arduino
The steps you need to take are simple. This is written for the ESP8266-01 but you can find the pinout for other models easily and use the same pins. First we will connect the Arduino UNO to a breadboard:

1. Connect the Arduino’s 3v3 **(3.3V)**  on a breadboard. The ESP8266 works with 3.3V and not 5V, so this is necessary. If you want to connect other components that use 5V, you can connect the 5V output of the breadboard, just make sure you don’t connect the two.

2. Connect GND (ground) to breadboard.

3. Connect the RES or RESET pin to ground. When you ground the reset pin, the Arduino works as a dumb USB to serial connector, which is what we want to talk to the ESP8266.

4. Connect the RXD pin of the Arduino to the RX pin of the ESP8266 .

5. Connect the TXD pin of the Arduino to the TX pin of the ESP (green color in the picture). Usually, when we want two things to talk to each other over serial, we connect the TX pin of one to the RX of the other (send goes to receive and the opposite). Here we do not have the Arduino talk to the ESP8266 though, our computer is talking to it via the Arduino.

6. Connect the GND pin of the ESP to the blue line and the VCC pin to the red line.
Finally CH_PD goes to the red line, supposedly it will not work if you do not connect this.

                                