# SODAQ Moja: Platform files for Arduino to run on ATmega328P

## What is it?

Everything you need to run Arduino on SODAQ Moja.  This SODAQ board
is compatible with Arduino Uno.

## Current state

Everything is there and has been tested.  It should work fine.

The platform is based on the optiboot bootloader.  Notice that we are
using our own version of optiboot. See https://github.com/SodaqMoja/optiboot.git
Optiboot uses only 512 bytes, 256 words, so that there is 32256 bytes
free for user code.

## Installation

1. Download the [ZIP File](https://downloads.sodaq.net/HardwareMoja.zip)
2. Unzip it in a folder called 'hardware' off your sketches directory,
   e.g. /home/kees/sketchbook/hardware/
   The ZIP file unpacks in a subdirectory called 'HardwareMoja', so the
   result must be in a directory like /home/kees/sketchbook/hardware/HardwareMoja
3. Restart the IDE !
4. Select Tools > Board > SODAQ Moja
5. To burn the bootloader, follow the Arduino [Bootloader](http://arduino.cc/en/Hacking/Bootloader) instructions.

## Requirements

* Works only on Arduino >= 1.5.x (tested with 1.5.8)
* There is a GIT branch arduino-1.0.x with the files for Arduino 1.0.x

## Supported Boards

* 'SODAQ Moja ATmega328P 8MHz at 57600 baud'
