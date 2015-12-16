Event Driven RGB Shield for Netduino
=============

![RGB LCD Shield Interrupt Pin](/../screenshots/images/RGBLCDInterrupt.jpg?raw=true "Optional Title")
This is a port of the Adafruit driver for the [Adafruit RGB LCD Shield](https://www.adafruit.com/products/714)
![RGB LCD Shield Kit](https://www.adafruit.com/images/1200x900/714-07.jpg)
## License
Check the [LICENSE.md](https://github.com/giawa/NetduinoRGBLCDShield/blob/master/LICENSE.md) file for the license associated with this code.
##About
The solution includes a program and class library that have been successfully tested on Netduino 2 and Netduino 3 WiFi.  Both the .sln and .csproj's are compatible with Visual Studio 2013 and set to use .Net Micro Framework 4.3. This solution provides an example on how to utilize Events (as opposed to a loop) to monitor button press feedback. This method allows Main() to exit so that other events (such as Serial Port Data Recieved) can be fired.  
##Usage
Simply solder a wire (pictured above) to Pin 20 (aka INTA) of the [MCP23017](https://www.adafruit.com/products/732) chip and then connect it to a digital I/O port on the netduino.  The example code uses GPIO_PIN_D10 to register the interrupt and read the data containing which button was pressed.
