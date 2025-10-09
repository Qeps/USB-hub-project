Four-layer PCB project expanding two USB ports from a computer into eight downstream ports.
Designed in KiCad, conceptually based on the CircuitDigest project, but extended to support two independent USB hub controllers.

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
