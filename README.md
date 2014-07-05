# SODAQ Mbili: Platform files for Arduino to run on ATmega328P

## What is it?

Everything you need to run Arduino on SODAQ Moja.  This SODAQ board
is compatible with Arduino Uno.

## Current state

Everything is there and has been initially tested.  It should work
fine.  There is more detailed testing which must be completed before
calling it completely 'done' though.  But that's how things work :-)

The platform is based on the optiboot bootloader.  Notice that we are
using our own version of optiboot. See https://github.com/SodaqMoja/optiboot.git
Optiboot uses only 512 bytes, 256 words, so that there is 32256 bytes
free for user code.

## Installation

1. Download the [ZIP File](https://downloads.sodaq.net/HardwareMoja.zip)
2. Unzip it in a folder called 'hardware' off your sketches directory,
   e.g. /home/kees/sketchbook/hardware/
   The ZIP file already unpacks in a subdirectory called 'sodaq-mbili'.
3. Restart the IDE !
4. Select Tools > Board > SODAQ Moja
5. To burn the bootloader, follow the Arduino [Bootloader](http://arduino.cc/en/Hacking/Bootloader) instructions.

## Requirements

* Works only on Arduino >= 1.0.5

## Supported Boards

* 'SODAQ Moja ATmega328P 8MHz at 57600 baud'
