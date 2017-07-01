# 18650-pi
A GPIO (but not HAT) 18650 battery charger and boost converter for the Raspberry Pi. 

Designed Archie Roques July 2017 - released under Attribution-NonCommercial-ShareAlike 4.0 International. 

## Why?
A conversation with a fellow maker sparked this project - there was not an elegant solution available for powering a Raspberry Pi from a common 18650 battery.
Now there is!

## What?
This PCB hangs off the Raspberry Pi, and connects to the GPIO pins via a 2\*20 pin header. The header is surface mount, but there are holes in the PCB design to allow it to slot on to the Pi's existing headers before a HAT or other board is placed on top. 
It contains an 18650 battery holder, all the circuitry necessary to charge the cell, and boost its voltage to the 5v required of the Raspberry Pi. 
It also contains a switch, to swap between charging and powering mode. This means you *can't use it as a UPS type board or swap between power sources on the go. **DO NOT CONNECT USB POWER AND BATTERY POWER AT ONCE - Things will burn!***
There is a microUSB port for charging and some indicator LEDs too. 

## How?
The board uses a U1V10F5 (AKA TPS6120X) boost converter, and a common TP4056 charger chip - this is what's on most cheap LiPo charger boards. 
The battery holder used, a Keystone Electronics 1043, has a slot down the middle, intended that the battery sits flat on the board. To save space, some components are placed in this gap, so the cell probably won't sit quite flush. 
The board is made for single sided SMD assembly, with the battery holder as a through-hole part (easy to solder with just 2 large connections).

### *NOTE: This is highly experimental! It ain't quite done, and it certainly hasn't been tested. Use it at your own risk - I am not responsibe for any damage you or it may do!*
