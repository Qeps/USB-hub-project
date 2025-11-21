# PCB Design
Four-layer PCB project expanding two USB ports from a computer into eight downstream ports.
Designed in KiCad, conceptually based on the CircuitDigest (Original project: https://circuitdigest.com/electronic-circuits/diy-hub-port-extender) project, but extended to support two independent USB hub controllers.

Base Project (CircuitDigest)
- Uses the GL850G USB 2.0 hub controller
- Expands one USB port into four downstream ports
- Powered directly from 5 V USB input
- The controller integrates internal 3.3 V and 1.8 V regulators, no external LDO required
- Basic passive components: resistors and decoupling capacitors
- USB-A connectors for downstream ports and one upstream connector
- Includes ESD protection (TVS diodes) for both upstream and downstream ports

Extended Version (this project)
- Two upstream USB inputs expanded to eight downstream ports (two hub controllers)
- Implemented on a 4-layer PCB for improved power and signal routing
- Thickened power traces for stable 5 V distribution across all ports
- Matched USB data line lengths to maintain signal integrity and timing
- Guard ring added around USB signal area to improve EMI and ESD immunity
- Independent hub sections sharing common 5 V supply and ground planes

KiCAD schematic:
<img width="1147" height="790" alt="image" src="https://github.com/user-attachments/assets/2c71ca67-29ca-43d0-8a9f-403946df93ee" />
<img width="1150" height="792" alt="image" src="https://github.com/user-attachments/assets/d400b812-4cdc-4ad3-a8a2-9c005e303023" />

KiCAD 3D board view:
<img width="1724" height="930" alt="ProjektUSBHUB" src="https://github.com/user-attachments/assets/7ac1dd4f-7ce7-4037-aa00-b9dce68094b5" />

# Prototype Board
This project is currently under development and PCBWay provided the prototype boards as part of a collaboration. The PCBs arrived with consistent manufacturing quality: clean routing, correct layer alignment, and accurate silkscreen. 

The ordering workflow was straightforward. Uploading the Gerber files and selecting the manufacturing parameters was clear enough that the whole process stayed focused on the technical aspects of the design.

Photo of the prototypes:
![20251121_185347](https://github.com/user-attachments/assets/3d8be624-a609-4d14-b512-eb19e8e2adbe)

Having the boards early in the process accelerates testing and helps refine the next revision.
Here you can order your board: https://www.pcbway.com/
