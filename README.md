# rattlemebonez32

### A 32 key monoblock with minimal choc spacing and vibes

This pocket board is the bigger cousin to the [idawgz32](https://github.com/ChrisChrisLoLo/idawgz32). Same minimalist key layout, more egonomic form factor. Uses a CH552 as its MCU, and runs FAK firmware.

![a photo of a rattlemebonez32](https://raw.githubusercontent.com/ChrisChrisLoLo/rattlemebonez32/main/images/PXL_20240408_002959511.jpg)

# Status
PCBs include a choc variant and a ks33 variant. Both work, though I highly recommend the choc variant as it's much easier to
assmble (ks33 switches do not snap into the board, making soldering difficult but possible).

The keys on this board are minimally spaced (15mm x 15mm), and as such will need special keycaps. 

This repo has a minimally spaced choc keycap based on the Philidelphia minimalist. You will likely need a 3D printer such as a Bambu Lab A1/A1 mini/P1P/P1S and set the slicing layer resolution to 0.08mm for best results. Printers like the Prusa i3/mini may also work, but have not been tested.

# Case
The case files can be found in the `case` directory.

The case comes in two parts, the top section and the bottom section.

## PCB
You can find the PCB source files in the `pcb` folder. The BOM files can be found in this folder.

![rattlemebonez pcb](https://raw.githubusercontent.com/ChrisChrisLoLo/rattlemebonez32/main/images/PXL_20240225_2PXL_20240408_00331990024453990.jpg)

## Directory Structure
- `case`
    You can find the files you need in this folder to print out a case and choc switches for the keyboard
- `drafts`
    Stores any ergogen or intermediate information used in making the case
- `pcb`
    Kicad project relating to the project. Contains the BOM, placement files, and gerbers
   
## BOM
- 1 PCBA
  - The PCB will include all electrical parts required, including switches.
- 1 Aluminum CNC upper case or 3DP upper case (technically optional, but strongly recommended)
- 1 Alumminum CNC lower case or CNC lower case
- 12 3mm M1.6 screws (go for flathead for a more flush fit, though other head types should also work)
- 8 1-2mm bumpons (something like Sj5302 is a good place to start)

## Assembly
Flash the pcb with my FAK branch (see below section). Bootmagic is enabled, so using the top left key to flash from here on out is doable.

Pop the 3D printed buttons/keycaps into the case. and screw the bottom case to the PCBA. Then place on the top and screw the top case to the PCBA.

Finally, place on the rubber bumpons

![rattlemebonez assembly](https://raw.githubusercontent.com/ChrisChrisLoLo/rattlemebonez32/main/images/PXL_20240408_003319900.jpg)

## Firmware
Branch and fork of FAK Firmware can be found here:
https://github.com/ChrisChrisLoLo/fak/tree/rattlemebonez32