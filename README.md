# ESP8266 - How to wire, flash and use an esp8266 with the Flipper Zero
First of all you have the pinout for the ESP8266 <br><br>
![ESP8266 PINOUT](https://github.com/Dankof04/esp8266/blob/main/ESP8266-Pinout-NodeMCU.png) <br><br>
We will use only four pins:<br><br>
           *  **VIN**: This pin is used to provide an external power source to the module when the power is not supplied through the USB port; in our case, the 5V pin in the Flipper Zero <br><br>
           *  **GND**: This pin provides a return path for the current, completing the electrical circuit.<br><br>
           *  **TX**: In a UART system, the TX pin is used to transmit data serially to another device that is listening on the RX (Receive) pin.<br><br>
           *  **RX**: In a UART system, the RX pin is used to receive serial data sent by another device that is transmitting on the TX (Transmit) pin.<br><br>
