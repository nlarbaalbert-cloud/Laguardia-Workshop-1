<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

This project implements a two-input AND gate.
Input A is ui[0] and input B is ui[1].
The result appears on uo[0].
The output is high only when both inputs are high.
This is a combinational circuit and does not use a clock or reset.
Unused outputs are not part of the demonstrated function.

## How to test

In Wokwi, start the simulation and toggle switches 1 and 2.
Test all four combinations and compare the LED with this table:

| A / ui[0] | B / ui[1] | Result / uo[0] | LED |
| --- | --- | --- | --- |
| 0 | 0 | 0 | Off |
| 0 | 1 | 0 | Off |
| 1 | 0 | 0 | Off |
| 1 | 1 | 1 | On |

The LED should light only for A = 1 and B = 1.

## External hardware

The Wokwi simulation uses two input switches and one LED.
The LED anode connects to OUT0 and the cathode connects to ground.
These components are simulation controls and indicators outside the chip.
No external hardware is needed to generate or inspect the GDS file.
