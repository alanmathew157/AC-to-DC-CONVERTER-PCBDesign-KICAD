[![Made with KiCad](https://img.shields.io/badge/Made%20with-KiCad-blue?logo=kicad&logoColor=white)](https://www.kicad.org/)
# AC to DC Converter PCB Design using KICAD -ALTIMUM
## PCB TOP VIEW
![PCB TOP VIEW](FrontSide.png)
## PCB BOTTOM VIEW
![PCB BOTTOM VIEW](BackSide.png)

## Project Overview
This PCB Design a  AC to DC converter that converts 220–240V AC mains into a regulated 5V DC output using a capacitive dropper method. The AC input first passes through C4 (2.2µF), which limits the current using capacitive reactance instead of a bulky transformer, while R3 (1Ω) reduces inrush current and protects the circuit from sudden surges. The reduced AC voltage is then converted into pulsating DC by a bridge rectifier made of D1–D4 (1N4007). After rectification, C2 (1000µF) smooths the ripple in the DC voltage and C1 (0.1µF) filters high-frequency noise to provide a cleaner supply. Zener diodes D5 and D6 offer over-voltage protection, and R1 and R2 (20kΩ) help stabilize the circuit. The filtered DC is fed into the L7805 voltage regulator, which provides a steady 5V output, while C3 (470µF) improves output stability. Finally, R4 (2.2kΩ) limits current to LED D7, which indicates that the power supply is ON, and the regulated 5V is available at the output terminal. Since this is a non-isolated design directly connected to mains voltage, it must be handled with great care. This project is my first attempt at learning KiCad and understanding transformer-less power supply design.

