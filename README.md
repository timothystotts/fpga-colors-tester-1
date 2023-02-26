# fpga-colors-tester-1

FPGA Colors Palette Tester Version 1
by Timothy Stotts

Note that this project is deprecated. The most recent project, with wider
hardware support and occasional updates, is Version 3 and is located at:
[fpga-colors-tester-3](https://github.com/timothystotts/fpga-colors-tester-3)

## Description
A small FPGA project of Xilinx IPI-BD with Microblaze CPU implementations for testing
24-bit color palette mixing of discrete RGB LEDs versus 16-bit color palette mixing of
a 96x64 OLEDrgb display's text.
The design targets the Digilent Inc. Arty-A7-100T FPGA development board containing a Xilinx Artix-7 FPGA.
Two peripherals are used: Digilent Inc. Pmod KYPD, Digilent Inc. Pmod OLEDrgb.

The folder Color-Tester-Design-AXI contains a Xilinx Vivado IP Integrator plus
Xilinx SDK design. A Microblaze soft CPU is instantiated to talk with board components,
a 4x4 alphanumeric keypad,
and 96x64 pixel color display.
A Xilinx SDK project contains a very small Standalone program in C; drivers
for the peripherals; and a main loop to repeatedly read keypad entry and then update both
discrete LEDs and display.


### Project information document:

[FPGA Colors Palette Tester info](https://github.com/timothystotts/fpga-colors-tester-1/blob/main/Colors%20Palette%20Tester.pdf)

### Target device assembly: Arty-A7-100T with Pmod KYPD, Pmod OLEDrgb, on extension cables
![Target device assembly](https://github.com/timothystotts/fpga-colors-tester-1/blob/main/Color-Tester-Design-Documents/img_color-palette-tester-assembled-20200831_202137119.jpg)

### Target device execution example: Arty-A7-100T with Pmod KYPD, Pmod OLEDrgb, on extension cables
![Target device execution example](https://github.com/timothystotts/fpga-colors-tester-1/blob/main/Color-Tester-Design-Documents/img_color-palette-tester-executing-a-20200831_204635464.jpg)
