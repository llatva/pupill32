# pypill32
## Compact and inexpensive USB-C development board for PY32F030 (TSSOP20) 32-bit MCU

*NOT YET TESTED -- I'll update this README once prototypes arrive*

## Features

* development/evaluation board for Pyua PY32F030F1xP8 MCU (TSSOP20)
* USB serial (CH340N, ESD protection)
* USB bootloader support (PUYAISP)
* 48 MHz operation with internal oscillator
* option for 32.768 kHz crystal (if used, pins PA9 and PA10 reserved)
* all peripheral pins available
* SWD header for programming, but if using USB bootloader, those pins can also be configured for other purposes
* 3V3 linear regulator; 3V3 logic levels
* powered from USB (SMD fuse for overcurrent protection)
* PWR LED and user-programmable USR led (activated by solder bridge)
* RESET and BOOT buttons

## Bootloader access

USB UART is connected to PA2/PA3 (TX/RX). To access bootloader (PUYAISP, USB-to-serial), either

* Disconnect USB cable, press and hold BOOT buttonm then connect the cable.

OR 

* Connect USB cable, press and hold BOOT button and press and release RESET button

## Independent project -- no affiliation or endorsement

This project is no way affiliated with Puya Semiconductor or any other commercial body. This is an indie evaluation board designed and built by a hobbyist. You may use this open hardware design, at your own risk, according to its license conditions, see the following chapter. 

## License

This board is licensed under CERN Open Hardware License, version 2, CERN-OHL-W (weakly reciprocal). 

Please refer to LICENSE file for more information.
