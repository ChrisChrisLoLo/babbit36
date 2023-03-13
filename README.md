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
| Part | Count | Notes |
|------|---------------|----------|
| PCB | 1 |  |
|Kailh Choc Hotswap Switches |40+10|| 	
|LL4148 SMD Diodes |	40+10 |	This board uses SMD diodes exclusively. I found though-hole diodes often easily slipped around in a way such that the board was no longer able to fit inside the case|
|Seeduino XIAO nrf52|1||
|Rubber Feet 	|6+2| 	Any should generally work, though I'm using ~2.5mm thick ones, as they give more space for screw heads, as well as the magnetic connector I'm using|
|CNC Printed Case 	|1 	|You could use PCB printing services like PCBWay to make one in resin, though I haven't confirmed if they'd be durable enough to survive in transit|
|PCB/FR4 backplate | 1| For the back of the keyboard case. Can be found in the pcb folder |
|M2 4mm Screw |	6+3 |	Screws for the PCB and case. Be careful of the size of the screw head! the flatter the better!
