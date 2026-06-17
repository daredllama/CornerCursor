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

## Bill oF Materials

Full Bill of Materials located in BOM file.

## Notes


