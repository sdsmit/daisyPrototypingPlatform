# Daisy Prototyping Platform

This repo contains the necessary files to build a daisy seed powered digital effects prototyping platform for instrument level signals.

# HARDWARE

Use the EAGLE files to generate a gerber file which can be manufactured by PCB suppliers such as JLCPCB. The parts list is included in the eagle file, apart from capacitors and resistors you will also need:  
TL072 dual op-amp  
LM7805 voltage regulator  
2 on/off momentary switches - https://smallbear-electronics.mybigcommerce.com/momentary-spst-no-soft-touch/  
Daisy Seed  
6 10k potentiometers  
2 TS 1/4 inch jacks  
1 DC barrel negative power jack  
1n5817 Diode   
2 leds  
1590BB stompbox enclosure  

# SOFTWARE

If you choose to use oopsy daisy (gen~ to daisy compilation tool). Download and install the oopsy package (https://github.com/electro-smith/oopsy). Place '''daisyPrototypingPlatformExample.maxpat''' in /Max 8/packages/oopsy/examples and place '''daisy.PetalLED.json''' in Max 8/packages/oopsy/source.

1. Open '''daisyPrototypingPlatformExample.maxpat''' and make modifications to the enclosed gen~ patcher.  
2. Inside the max patch, select browse on the oopsy object and select '''daisy.PetalLED.json'''.  
3. Put your daisy into DFU and hit save. This will flash the daisy with your patch and the corresponding controls should be active.  
