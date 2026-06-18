**Reviewer, please look at the "FALLOUT VIDS" folder to count the hours from those videos. It should constitute about 16 hours.

# CornerCursor

A trackball mouse with 2 configurable buttons and a scroll ring. Made to be positioned on the corner of a laptop so that CADding is easier in any location.

Hardware created through Onshape. PCB made through KiCad. Firmware developed through VSCode.

## Features

- 3d printed case 
- Trackball navigation using PMW-3360 sensor
- Scroll Ring using # magnets with Hall Effect sensors
- 2 buttons
- Firmware designed for CAD use in Onshape

## Status

Currently unfinished. CAD, KiCAD, and Firmware are complete, but no actual model has been built. Debugging afterwards would also be expected.

## CAD Model

This is the overall build for the CornerCursor, which includes the case and the trackball.
Made using Onshape

<img width="1558" height="1322" alt="image" src="https://github.com/user-attachments/assets/c79a07fb-09e5-412f-86c7-eab63c71f8c0" />


## PCB

This is the schematic, PCB, and a render of the board. Note that the off-board component, such as the Hall effect sensor and USB-C connector, is not shown on the PCB> 

Schematic

<img width="2332" height="1568" alt="Screenshot 2026-06-17 145611" src="https://github.com/user-attachments/assets/5c84ca94-cb42-4110-ae21-5fae73257b7b" />

PCB

<img width="2044" height="952" alt="Screenshot 2026-06-17 145516" src="https://github.com/user-attachments/assets/61263968-4b0f-4952-80ab-dbfeeedf5c4e" />

Render

<img width="2228" height="1220" alt="CornerCursor" src="https://github.com/user-attachments/assets/693210bc-b677-47c3-9953-7c7f40fa677d" />


## Firmware

Firmware sets up a 2-button trackball mouse that uses a PMW3360 sensor and a scroll ring.

To flash the software onto the board, connect your device to the mouse. A RPI-RP2 drive should show up, at which point you can drag the given UF2 file. To flash it again, hold the BOOT button and press the RESET button on the board.

## Assembly

1. Solder the necessary parts on the PCB, using the schematic and PCB image as reference. (Remember PMW 3360 has a sensor)
2. Attach the board onto the bottom case using 2 M3X2 screws (They will go into plastic).
3. Wire the Hall effect sensor through the hole on the part named "top".
4. Attach the "top" part to the base case using 2 M3x8 screws.
5. Screw the two buttons to the bottom base using 4 M3x6 screws.
6. Attach the top case to the bottom case using 3 M3x12 screws.
7. Place the big bearing on the "top" part and attach neodymium magnets to the ring.
8. Place static bearings into divots in the "top" part and then place the trackball.

## Bill oF Materials

Full Bill of Materials located in BOM file.

## Notes

AI Usage in this project was used for research, such as tutorials and datasheets; none of the code or CAD is AI-generated

