# Daisy Prototyping Platform

This repo contains the necessary files to build a daisy seed powered digital effects prototyping platform for instrument level signals.

# HARDWARE

Use the EAGLE files to generate a gerber file which can be manufactured by PCB suppliers such as JLCPCB. Use the export feature to export a PDF drilling template for the potentiameters. All other parts (jacks switches and LEDS) are floating and are not included in the pcb layout. The parts list is included in the eagle file, apart from capacitors and resistors you will also need:  
- TL072 dual op-amp
- LM7805 voltage regulator
- on/off momentary switches(2) - https://smallbear-electronics.mybigcommerce.com/momentary-spst-no-soft-touch/  
- Daisy Seed - https://www.electro-smith.com/daisy/daisy
- 10k potentiometers (6)  
- TS 1/4 inch jacks (2)
- DC barrel negative power jack  
- 1n5817 Diode   
- LED(2)
- 1590BB stompbox enclosure  

The items should fit in this orientation.

![Alt text](images/front.jpg?raw=true "Title")
![Alt text](images/back.jpg?raw=true "Title")


# SOFTWARE

If you choose to use oopsy daisy (gen~ to daisy compilation tool). Download and install the oopsy package (https://github.com/electro-smith/oopsy). Place `daisyPrototypingPlatformExample.maxpat` in `/Max 8/packages/oopsy/examples` and place `daisy.prototypingPlatform.json` in `Max 8/packages/oopsy/source`.

1. Open `daisyPrototypingPlatformExample.maxpat` and make modifications to the enclosed gen~ patcher.  
2. Inside the max patch, select browse on the oopsy object and select `daisy.prototypingPlatform.json`.  
3. Put your daisy into DFU and hit save. This will flash the daisy with your patch and the corresponding controls should be active.  

It should also be possible to use daisySP with this platform. It has only been tested with oopsy and gen~.
