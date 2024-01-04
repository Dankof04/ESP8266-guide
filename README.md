# ESP8266 - How to wire, flash and use an ESP8266 with the Flipper Zero

# FLASHING
In order to use an ESP8266 attached to the Flipper Zero, we have to flash our ESP8266 with the program we want to execute. In my case, and the first version of this guide, we are flashing the [Wifi Scanner](https://github.com/SequoiaSan/FlipperZero-WiFi-Scanner_Module) on our ESP8266.

Flash your ESP8266 with the Wifi Scanner by following this steps:

  **1º**   Connect your ESP8266 to your computer using a Micro USB cable (in my case)
  
  **2º**   Put your ESP8266 into flashing mode (Hold the FLASH/BOOT button, then press the RESET button once and release the FLASH/BOOT BUTTON)
  
  **3º**   Go to the [Online Flasher](https://sequoiasan.github.io/FlipperZero-WiFi-Scanner_Module), select ESP8266 and flash your board with the Wifi Scanner (Make sure you don't have other site or program trying to use the serial port that your ESP8266 is using)

  **4º** Let's do the wiring!!!!

# WIRING

First of all, here is the pinout for the ESP8266 and the pinout for the Flipper Zero:

![ESP8266 PINOUT](https://github.com/Dankof04/esp8266/blob/main/ESP8266-Pinout-NodeMCU.png)
![FLIPPER ZERO PINOUT](https://github.com/Dankof04/esp8266/blob/main/FlipperZero_Pinout.png)

We will use only four pins:

- **VIN**: This pin is used to provide an external power source to the module when the power is not supplied through the USB port; in our case, the 5V pin in the Flipper Zero.
- **GND**: This pin provides a return path for the current, completing the electrical circuit.
- **TX**: In a UART system, the TX pin is used to transmit data serially to another device that is listening on the RX (Receive) pin.
- **RX**: In a UART system, the RX pin is used to receive serial data sent by another device that is transmitting on the TX (Transmit) pin.

The wirings between the ESP8266 and the Flipper Zero are:

- **VIN** (ESP8266) ----------------------------> **5V** (Pin 1 - Flipper Zero)

- **GND** (ESP8266) ---------------------------> **GND** (Pin 8 - Flipper Zero)

- **TX** (ESP8266) -----------------------------> **RX** (Pin 14 - Flipper Zero)

- **RX** (ESP8266) -----------------------------> **TX** (Pin 13 - Flipper Zero)

- **PC0** (Pin 16 - Flipper Zero) ---------------> **GND** (Pin 18 - Flipper Zero)

With this wiring you should be able to use the ESP8266 with your Flipper Zero

# SOLDERING
I've soldered my board using the [Official Prototyping Boards](https://shop.flipperzero.one/collections/flipper-zero-accessories/products/proto-boards).

There you have some photos of my prototype:

![PROTOTYPE FRONT](https://github.com/Dankof04/ESP8266-guide-not-finished-/blob/main/ESP8266_Front.jpeg)
![PROTOTYPE BACK](https://github.com/Dankof04/ESP8266-guide-not-finished-/blob/main/ESP8266_Back.jpeg)

# HOW TO USE WIFI SCANNER
We've soldered our prototype and flashed it with the Wifi Scanner.

Now we'll try our creation (Note: you need the WifiScanner.fap on your Flipper):

**1º** Search the Wifi Scanner app on your Flipper:

![Search the application](https://github.com/Dankof04/ESP8266-guide-not-finished-/blob/main/Step_1.png)

**2º** If the flashing was succesful, your Flipper will start searching for wifi networks:

![Flipper searching networks](https://github.com/Dankof04/ESP8266-guide-not-finished-/blob/main/Step_2.png)

**3º** When finished you'll see a screen like this one, where you can navigate through the wifi networks by pressing UP and DOWN buttons or LEFT and RIGHT as well:

![Network list](https://github.com/Dankof04/ESP8266-guide-not-finished-/blob/main/Step_3.png)

**4º** Press the OK button to start Monitor Mode, you'll see this screen:

![Monitor starting](https://github.com/Dankof04/ESP8266-guide-not-finished-/blob/main/Step_4.png)

**5º** Start monitoring the WiFi network:

![Monitoring](https://github.com/Dankof04/ESP8266-guide-not-finished-/blob/main/Step_5.png)


# If you have any questions, feel free to contact me via [Discord](https://discord.com/users/dankof.exe)https://discord.com/users/dankof.exe)


