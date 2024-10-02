## Adafruit RP2350 22-pin FPC HSTX to DVI Adapter for HDMI Displays PCB

<a href="http://www.adafruit.com/products/6055"><img src="assets/6055.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit RP2350 22-pin FPC HSTX to DVI Adapter for HDMI Displays. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/6055

### Description

You may have noticed that our RP2350 Feather has an FPC output connector on the end for accessing the HSTX (High Speed Transmission) peripheral. This new capability, not available on the RP2040, is specifically designed to allow the RP2350 chip drive DVI displays really easily! Historically you could use DVI on the RP2040 by mashing together some overclocking and a lot of PIO - it works but its quite hacky. The HSTX peripheral is streamlined, and doesn't require PIO or overclocking and there's a lot more RAM on the RP2350.

If you want to try out HSTX to drive an HDMI monitor or display, this dongle is what you need to take HSTX out and give you a connector with proper level shifting and signal conditioning. Simply connect a 22 pin FPC cable between the Feather RP2350 and Adafruit RP2350 22-pin FPC HSTX to DVI Adapter for HDMI Displays then load DVI output code. In CircuitPython, we have support for 320x240 pixels at 16-bit color, which gets pixel doubled to 640x480. Or, if you're willing to cut some colorspace to save RAM, you can get true 640x480 resolution at 4 / 8 bit color, or 1 / 2 bit grayscale.

The eight HSTX lines are connected to the differential Clock (IO #14 & 15), Lane0 (#18, 19), Lane1 (#16, #17), and Lane2 (#12, #13) connections. I2C is connected as well so you can read the display EEPROM. Hot-plug-detect is connected to IO #11 on the Feather, but can be disconnected by cutting a jumper on the bottom. Ditto for CEC which we connect by default to IO #10.

Each order comes with one DVI adapter board. 22-pin FPC cable is not included, so be sure to get one too!

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.
