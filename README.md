# ESP8266 - How to wire, flash and use an ESP8266 with the Flipper Zero


# FLASHING

# WIRING

First of all, here is the pinout for the ESP8266:

![ESP8266 PINOUT](https://github.com/Dankof04/esp8266/blob/main/ESP8266-Pinout-NodeMCU.png)

We will use only four pins:

- **VIN**: This pin is used to provide an external power source to the module when the power is not supplied through the USB port; in our case, the 5V pin in the Flipper Zero.
- **GND**: This pin provides a return path for the current, completing the electrical circuit.
- **TX**: In a UART system, the TX pin is used to transmit data serially to another device that is listening on the RX (Receive) pin.
- **RX**: In a UART system, the RX pin is used to receive serial data sent by another device that is transmitting on the TX (Transmit) pin.

The wirings between the ESP8266 and the Flipper Zero are:

- **VIN** (ESP8266) ----------------------------> **5V** (Pin 1 - Flipper Zero)

- **GND** (ESP8266) ---------------------------> **GND** (Pins 8, 12, or 18 - Flipper Zero)

- **TX** (ESP8266) -----------------------------> **RX** (Pin 16 - Flipper Zero)

- **RX** (ESP8266) -----------------------------> **TX** (Pin 15 - Flipper Zero)

With this wiring you should be able to use the ESP8266 with your Flipper Zero
