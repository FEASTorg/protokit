# Conn: USB Micro-AB with VBUS Circuitry

## info

Main functionality is to provide "VUSB circuitry" for AVR microcontrollers. Can also be used as generic uUSB breakout by shorting 68R resistor footprints or as breadboard power supply (supplying 5V).

Allows for supplying different voltages by populating the bottom side with desired regulator. The following modes are possible:

- Supply rail and Vcc pin with 5V directly from USB (regulator not populated, short all 3 pads of solder jumper)
- Supply regulator with 5V from USB which in turn supplies rail and Vcc pin (short center and top pad)
- Supply regulator from rail and get regulated voltage on Vcc pin (short center and bottom pad)

## parts dump

- [Molex - 0475900001 - CONN RCPT MICRO USB AB 5P SMD RA](https://www.digikey.ca/en/products/detail/molex/0475900001/1832254)
- [Amphenol ICC (FCI) - 10104111-0001LF - CONN RCPT USB2.0 MICRO AB SMD RA](https://www.digikey.ca/en/products/detail/amphenol-cs-fci/10104111-0001LF/2350354)
