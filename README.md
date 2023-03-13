# babbit36

A 36 key low profile wireless ortholinear board. Uses a Seediuno XIAO as the MCU, and runs on ZMK.
Featues:
  - Low Profile, uses CFX keycaps
  - Commodity parts, only non standard part is the shift register
  - Relatively affordable! 
    - Case only requires one CNC/3D Printed part and one FR4 backplate

## Note
This keyboard uses CFX spacing, and therefore requires Chosfox CFX keycaps, or keycaps with similar spacing.

## Status
v0 is functional and works as is!  

## PCB/CNC case

You can generate the gerbers from source in the pcb directory, and send off imediately to PCBWay or the like. There's one gerber for the keyboard and another gerber for the backplate of the case. There's also step files ready to use to order your own 3DP/CNC case. My CNC case was sponsored by PCBWay. I was a bit anxious about my CNC file since this is my most complicated keyboard case to date, but PCBWay did a fantastic job! I was very happy that the tolerances were good, that the finishing looked great, and that it was all at a great price given the complexity of the case! I highly recommend their services for CNC prototyping/manufacturing!

## BOM

The following is the materials you will want/need to make your own babbit36. Note that anything amount after a + denotes the rough amount of spares you may want to have when ordering the parts.
|Part|Count|Notes|
-------------------
|PCB |1|| 	

Kailh Choc Hotswap Switches 	40+10 	
LL4148 SMD Diodes 	40+10 	This board uses SMD diodes exclusively. I found though-hole diodes often easily slipped around in a way such that the board was no longer able to fit inside the case
1.8" ST7735 TFT 	1 	Generally speaking, you want the one with the Red PCB. Do NOT use the one from Adafruit, as the pin order on that one is different
Raspberry Pi Pico 	1 	Try to get the original or a very similar clone with castellated pins. From casual testing, other RP2040 boards may not work (for example, the Pico clones from WeAct can't seem to properly drive the LCD with 3.3V logic)
Rubber Feet 	6+2 	Any should generally work, though I'm using ~2.5mm thick ones, as they give more space for screw heads, as well as the magnetic connector I'm using
3D Printed Case 	1 	You could use PCB printing services like PCBWay to make one in resin, though I haven't confirmed if they'd be durable enough to survive in transit
M2 Nuts 	10+5 	6 nuts to hold the PCB to the case, and another 4 to hold the acrylic screen to the PCB. I'm using nylon nuts, though any should work. I recommend you grab this with a hex spacer kit, as you get all the M2 parts you need in a single purchase!
M2 8mm Double Female spacer 	4+2 	Spacers to keep the acrylic from the pcb
M2 12mm Screw 	4+2 	Screws for the acrylic screen
M2 6mm Screw 	6+3 	Screws for the PCB and case. Be careful of the size of the screw head! the flatter the better!
Acrylic Screen 	1 	You can cut one out using the svgs in the outlines folder
Design

See DESIGN.md for small insights about the design choices that went into this board.
Directory Structure

    case You can find the files you need in this folder to print out a case for the keyboard
    drafts Stores any KLE or intermediate information used in making the case
    firmware Used to store any firmware relating to the keyboard. Merges to the QMK repo planned.
    outlines Outlines used for the acrylic screen. Use these to cut your own!
    pcb Kicad project relating to the project
