# PCB Files

## 701C USB Hub
An internal 4-port USB hub that sits on the left side of the mainboard. It exposes two external USB3 Type A ports, one internal USB3 Type A port (intended for a Logitech Unifying Receiver), and a gigabit ethernet port.
**NOTE: This design is untested.**
## Breakout boards
A collection of various breakout boards used during development.
## eDP Adapter
An adapter that converts the Framework's embedded DisplayPort interface to an iPad 7 panel. It has a passthrough for four lanes of DP and the backlight driver.
## Input Cover Flex
Flex circuit that jumps from the Framework input cover connector to the KB-Mouse Interface board.
## KB-Mouse interface
This is the rug the ties the room together, as it were. It houses the following items:
* Teensy 3.6 dev board that allows the keyboard and trackpoint to appear as USB devices
* Sprintek 8707 Trackpoint to PS/2 amplifier
* Hall effect sensor to provide feedback on lid closure (using a magnet glued to the bottom of the butterfly keyboard mechanism)
* M.2 connector fed from the "M.2 Breakout" PCBA
* FETs to drive the original LED indicators and a connection to the "LED Bar" PCBA.
* Passthrough for the Framework audio board (this is required since the audio board houses the factory lid sensor circuit)
* Power button connector
## LED bar
Carrier board for the original 701C LED indicator bar. This LED bar is seemingly bespoke to the 701C, so it was salvaged from a broken laptop.
## M.2 Breakout
Converts all the signals on the mainboard's M.2 port to a fine pitch FFC cable, allowing it to mate with the "KB-Mouse Interface" board.
## Power button
Lil' board to hold a momentary pushbutton on the right side of the chassis. This board and its mounting post also doubles as the retaining mechanism for the "M.2 Breakout" board.
## USB U-Turn
Allows the "701C USB Hub" board to mate with the Framework mainboard. It's essentially a super low profile 180 degree USB Type C male to USB Type C male "cable."
**NOTE: This design is untested and is a complete affront to all things impedance matching.**