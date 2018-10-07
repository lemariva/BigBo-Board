# BigBo-Board

BigBo is a multi-target board for Energy Metering & Power Monitoring. It's the big brother of [PiCoBo](https://github.com/lemariva/PiCoBo-Board). I designed it using the MSP430F5529LP that is part of the MSP430 Texas Instruments family of low-power microcontrollers.

More info will be available on https://lemariva.com soon.

## Components
The board includes:
* CP2102 for UART communication (with ESD-Protection)
* Socket for a NRF24L01 module
* CD4504B: level shifter
* BQ27510-Q3: battery fuel gauge
* BQ24210DQCT: Li-Ion battery charger
* CAT24FC32UI: EEPROM memory
* TPS6300x: buck-boost converters (for 5V)
* MCP39F501: power-monitoring
* etc.

This board is a Energy Metering & Power Monitoring demonstration board with communication possibilities (0.1% error across 4000:1 dynamic range). I designed it near 2013, when home solutions were limited and expensive. The power energy metering & power monitoring functions are based on the [ARD00455](https://www.microchip.com/Developmenttools/ProductDetails/ARD00455) board.

The board can be supplied using:
* a battery (Li-Ion) which can be also charged
* 5V over the micro-usb connector
* 230V AC (not a typo error - 230V AC!). The floating 3.3V is generated using a LM1117. Check the HIGH-Voltage page on the schematic.

Additionally multiple pinouts are available to connect external sensors (e.g. DHT11), servo motors, LEDs etc. For testing uses it can be programmed using the MSP430F5529LP LaunchPad.

## PCB
![PCB Board Top Side](https://raw.githubusercontent.com/lemariva/BigBo-Board/master/pics/bigbo_top_side.png)
![PCB Board Bottom Side](https://raw.githubusercontent.com/lemariva/BigBo-Board/master/pics/bigbo_bottom_side.png)

### Applications
* Energy Metering & Power Monitoring
* Smart switch
* Sensor measurement (Temperature etc.)
* LEDs control
* Communication
* etc.

### Revision
* 1.0 first version

### Disclaimer
Use at your own risk and be careful specially with the 230V AC part.

I ordered the board (I have 10 PCBs over here) but I didn't have enough time to solder the components. I've checked the design many times but errors could be over there. I'll be updating the code that I had for the board soon.
