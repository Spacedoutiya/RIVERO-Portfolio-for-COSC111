## Laboratory Activity 1

## Objectives:
• To apply digital signal control in an Arduino-based circuit.
• To develop a sequential LED lighting system where LEDs are activated and deactivated in a predefined order. The system should also allow modifications to independently control odd or even-numbered LEDs.

## Overview:
This laboratory exercise involves constructing an Arduino circuit incorporating five LEDs, each connected through resistors to an Arduino Uno board. The objective is to program the LEDs to turn on and off sequentially with a brief delay between transitions.

To execute the experiment, the LEDs must first be correctly wired to the Arduino, following the reference diagram in act1.png. After ensuring proper connections, the provided code should be uploaded using the Arduino IDE. It is essential to verify that the correct communication port is selected before running the program. Once executed, the LEDs will illuminate in a sequential pattern with a one-second delay between each transition.

For additional functionality, modifications can be made to control only the odd- or even-numbered LEDs by adjusting the loop function in the code. The respective code variations for these patterns are available in the provided .ino file within the project folder.

## Key Programming Concepts:
- LED Pin Configuration (ledPins[]): An array storing the pin numbers corresponding to each LED.
- Total LED Count (numLeds): Defines the total number of LEDs in the setup. 
- Setup Function: Initializes each LED pin as an output to ensure proper control.
- Loop Function: Implements the logic for sequentially turning LEDs on and off according to the specified pattern.
