# lx-sw-btn

![lx-sw-btn](/pictures/lx-sw-btn.png)

This repository contains the KiCad project for the "lx-sw-btn": a 2HP eurorack module with 4 customizable switches enabled CV outputs!

With two buttons and two switches, the lx-sw-btn enables four CV "on-off" outputs. By default, the output is set to 0-5V, but each output can be fine-tuned through front-panel adjustment holes ranging from -10V to +10V. This will allow you to use the switches not only as triggers but also for precise CV control.

The module is extremely compact with only a single PCB featuring SMD components on both sides, ensuring no wasted space!

I used [PCBWay](pcbway.com) services were used for the PCB manufacturing, both pcb and front panel.

## Content

Under the [hardware](/hardware/) folder, you will find the KiCad project with the following files:

- [Project](/hardware/2hp-simple-switch-button/2hp-simple-switch-button.kicad_pro)
- [Schematic](/hardware/2hp-simple-switch-button/2hp-simple-switch-button.kicad_sch)
- [Main PCB](/hardware/2hp-simple-switch-button/2hp-simple-switch-button.kicad_pcb)
- [Front panel PCB](/hardware/2hp-simple-switch-button/2hp-simple-switch-button-front-panel.kicad_pcb)

## Circuit

![schematic-exerp](/pictures/schematic-op-amp.png)

The circuit consist of 4 times the circuit below: an opamp as follower with a voltage devider between VCC and VEE as input through a potentiometer. The output is set to 1k impedance with a RC filter useful for debouncing the switches and buttons.

The module also have power supply invert polarity protection and input filtering.
