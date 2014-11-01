Hackscribble FRAM Hardware
==========================

#### *PCB designs for connecting Fujitsu MB85RS Ferroelectric memory (FRAM) to Arduino.*

Created on 20 April 2014 by Ray Benitez  
Last modified on 1 November 2014 by Ray Benitez		
  
These hardware designs are licensed by Ray Benitez under the Creative Commons Attribution-Sharealike 4.0 International License.
	
git@hackscribble.com | http://www.hackscribble.com | http://www.twitter.com/hackscribble


### About the hardware

#### Level converter circuits

These circuit snippets connect 3.3V MB85RS FRAM chips to 5V Arduino inputs / outputs.  

Two design approaches are shown:

1. Discrete design using BSS108 FETs, following the approach used by the Adafruit level converter.

2. Integrated design using TXB0104 to reduce PCB space required. 

The designs are in Eagle format.

Note: These circuits have not yet been verified in hardware.

#### Mini-shield

The mini-shield allows up to three 3.3V FRAMS to be connected to an Arduino (or an LPCXPresso board).  It uses an extended version of the integrated circuit snippet (above) using a TXB0108. The board has been tested with Arduino Uno and LPCXpresso 11U68 boards.

The design is in KiCad format.

Note: There are two voltage select solder jumpers on the board.  Only the 3.3V jumper should be closed; the 5V jumper should be left open. The SPI bus solder jumpers should also be left open. 

The REVISION A board also includes test points for monitoring the SPI bus.
<br>

<hr>


### Change history

#### 1 November 2014

Added mini-shield REVISION A.

#### 20 April 2014

Initial release of level converter circuits REVISION A.
