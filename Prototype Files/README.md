# PROTOTYPE INFORMATION:

## Parts:
- Arduino Pro Micro [ATMega32u4]
- TEMT6000 Light Sensor (This sensor has terrible resolution, find a better one in the future)
- TP4056 Charging Module
- Mystery Feature Phone Battery
- 128x64 I2C OLED Display
- 3x 6mm Button Switches

## Details:
Code only has apperture priority mode.
Aperture is changed by buttons on the left.
Reading is taken with button in the right.
IEV & LUX are updated every 75ms.

IEV is a slightly modified version of EV to compensate for a more accurate exposure.
Rounding up after half of the required LUX for the next EV is being read.
Also this fixed the flickering of a 'borderline' EV.
