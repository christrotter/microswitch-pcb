# microswitch-pcb
Designed for use on the [ArcPedals mk2](https://github.com/christrotter/qmk_firmware/tree/arcboard-series/keyboards/handwired/arcpedals_mk2) - with the accompanying files, a drop-in replacement for the old MX-based switches.

JLC wanted to charge me extra for using SK6812-MINI-E leds, so I swapped over to the SK6805 and tripled the led count.  As one does.

<a href="images/button-inator.jpg"><img src="images/button-inator.jpg" width="800"/></a>

# Overview
Only items of note - the pour is on the top layer only, and I tried to make it as friendly for manufacturing and human usage as possible.

<a href="images/pcb-overview.jpg"><img src="images/pcb-overview.jpg" width="800"/></a>

<a href="images/pcb-assy-cutaway.jpg"><img src="images/pcb-assy-cutaway.jpg" width="800"/></a>

## Parts
Gerbers, bom, position files and more in the releases section.

- 0402 100nF multilayer ceramic capacitor
- SOD-123F 1N4148W diode
- Omron D2F-L microswitch (key point, plunger only; heavier spring cuz feet)
- JST-XH-2.54 horizontal (or vertical, up to you) 6-pin connector
- 3x SK6805-EC15 LEDs

# Schematic overview
Pretty straightforward.
- 2.54 header (I designed for JST-XH 2.54 horizontal)
- 5v/GND power system w. 100nF capacitor
- LED signal via DI/DO pins
- 'key' signal via IN/OUT pins w. default diode on return leg
  - optionally cut the 2/3 bridge trace and solder pads 1/2 together for the direct pin (to GND)

<a href="images/pcb-schematic.jpg"><img src="images/pcb-schematic.jpg" width="800"/></a>

# 3d view
<a href="images/pcb-3d-front.jpg"><img src="images/pcb-3d-front.jpg" width="400"/></a>
<a href="images/pcb-3d-back.jpg"><img src="images/pcb-3d-back.jpg" width="400"/></a>
