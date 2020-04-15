<a href="https://www.microchip.com" rel="nofollow"><img src="images/Microchip.png" alt="MCHP" width="300"/></a>

# AVR128DA48 LED Blink Using Timer Interrupt Code Example

This repository provides an Atmel Studio solution with a bare metal code example for an LED blink driven by a timer overflow interrupt (Timer/Counter Type A).
This example demonstrates a simple toggling of a LED connected to the PC6 (on-board user LED) with an on/off cycle period of 1 second implemented through the use of an interrupt generated by the overflow of TCA0. The on-board user LED on the development board will toggle each 500 milliseconds.

## Related Documentation
More details and code examples on the AVR128DA48 can be found at the following links:
- [AVR128DA48 Product Page](https://www.microchip.com/wwwproducts/en/AVR128DA28)
- [AVR128DA48 Code Examples on GitHub](https://github.com/microchip-pic-avr-examples?q=avr128da48)
- [AVR128DA48 Project Examples in START](https://start.atmel.com/#examples/AVR128DA48CuriosityNano)


## Software Used
- Atmel Studio 7.0.2397 or newer [(microchip.com/mplab/avr-support/atmel-studio-7)](https://www.microchip.com/mplab/avr-support/atmel-studio-7)
- AVR-Dx 1.0.18 or newer Device Pack


## Hardware Used
- AVR128DA48 Curiosity Nano [(DM164151)](https://www.microchip.com/Developmenttools/ProductDetails/DM164151)

## Setup
The AVR128DA48 Curiosity Nano Development Board is used as test platform
<br><img src="images/AVR128DA48_CNANO_instructions.PNG" width="500">

The following configurations must be made for this project:

|Pin           | Configuration      |
| :----------: | :----------------: |
|PC6 (LED0)    | Digital Output     |


## Operation

1. Open the *AVRDA_LED_blink_interrupt.atsln* solution in Atmel Studio

2. Build the solution: right click on *AVRDA_LED_blink_interrupt* solution and select Build
<br><img src="images/AVR-DA_LED_blink_interrupt_build.png" width="500">

3. Select the AVR128DA48 Curiosity Nano on-board debugger in the *Tool* section of the project settings:
 - Right click on the project and click *Properties*;
 - Click *Tool* tab on the left panel, select the corresponding debugger and save the configuration (Ctrl + S)
<br><img src="images/AVR-DA_LED_blink_interrupt_tool_settings.png" width="500">


4. Program the project to the board: select *AVRDA_LED_blink_interrupt* project and click *Start Without Debugging*:
<br><img src="images/AVR-DA_LED_blink_interrupt_program.png" width="500">

Demo:
<br><img src="images/AVR-DA_LED_blink_interrupt.gif" width="500">

## Summary
This example represents a basic LED toggling application. The toggling is implemented using the built-in delay function and the on-board LED of the AVR128DA48 Curiosity Nano is toggled every 500 milliseconds.
