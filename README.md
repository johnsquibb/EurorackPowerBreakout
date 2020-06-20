# EurorackPowerBreakout
Eurorack 10-pin power breakout, designed to fit a standard breadboard.

## Features
- Designed for use with 10 pin keyed horizontal box header.
- Fits standard breadboard with attached bus bars having 0.1" lead spacing.
- +/-12V with button power on/off (optional)
- LED indicators (optional).
- 10uF local power bypass (optional) 

## Usage
The breakout board is designed to be placed on the left-hand or right-hand side of a standard 0.1" breadboard. For the left-hand orientation, the -12V connection will be on the top power bus rail, and +12V on the bottom. This coincides with the power pins of a left-hand orientation of a TL074 op amp IC package that I frequently use (pins 4 and 11). See [image](./image/eurorackPower10pin_breadboard.jpg) for a visual reference.

The LEDs are optional, and can be omitted and/or replaced with extra header pins. I use the convention of red for +12V and yellow for -12V. I use a minimum of 1k ohm resistors for LEDs, but higher values may be used to reduce the brightness.

The DPDT power button is optional and can be replaced with header pins and jumpers, or omitted entirely. If omitted, pins 2 and 3 must be bridged for `DPDT_A` and `DPDT_B` connections (Note: pin 1 is identified by square pad).

The power bypass capacitors are optional and can be omitted without modification to the circuit. I recommend using at least 50V capacitors for +/-12V Eurorack power connections. I've linked my preferred caps below in the Bill of Materials, as they are short and less susceptible to bending when handling the board.

## Bill of Materials
All through-hole components.

Here's a list of some of the specialized parts:

- [10 PIN BOX HEADER CONNECTOR 2.54MM RIGHT ANGLE](https://www.taydaelectronics.com/10-pin-box-header-connector-2-54mm-right-angle.html)
- [DPDT 8x8mm](https://www.taydaelectronics.com/push-button-switch-latching-on-off-dpdt-0-5a-50vdc-8x8mm.html)
- [3mm LED (yellow)](https://www.taydaelectronics.com/led-3mm-yellow.html)
- [3mm LED (red)](https://www.taydaelectronics.com/led-3mm-red.html)
- [10uF Electroylitic Capacitors](https://www.digikey.com/product-detail/en/nichicon/UMT1H100MDD/493-15562-ND/2598786)

See the [interactive BOM](./bom/ibom.html) document for interactive visual guide.

## License
Schematic and PCB designs by John Squibb are licensed under MIT (see LICENSE).

All other software dependencies are the copyright of their respective owners.

See KiCad and InteractiveHtmlBom projects for their software licenses:

* [https://github.com/KiCad](https://github.com/KiCad)

* [https://github.com/openscopeproject/InteractiveHtmlBom](https://github.com/openscopeproject/InteractiveHtmlBom)
