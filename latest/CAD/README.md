## Board design files

This directory contains Eagle CAD files as well as schematic PDFs and Gerber exports for board fabrication.

The board stackup is good enough for either OSH Park 4-layer, or JLCPCB 4-layer with controlled impedance (JLC2313). 

### Latest Board
Revision 10.0.1 is latest. It adds a few safety features such as ESD protection and isolation between the board's MCU pins and the outside world.
An appropriate breakout board for series 10.x is included. The "TX OFF" signal is now buffered by a MOSFET on the transponder board and the
logic is inverted.

The LED "status" signals are now current-limited open drain outputs via N-Channel MOSFETs on the transponder board. This means they could work
with any voltage up to 16V without risk of damage to the MCU.

### Older Boards
Revision 9.3.0 is not bad. I built it at JLCPCB with the exact gerber files I posted here. It is fully functional and performed as expected,
with some caveats (no ESD protection, no reverse polarity protection)

The 9.3 board adds 3 "status" signals that can drive LEDs (with appropriate current limiting resistors!). These are optional.



