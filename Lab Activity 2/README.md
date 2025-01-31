## Lab Activity #2

## Objectives:
- To explore the concept of analog signals and their application in an Arduino circuit.
- To understand the process of converting analog signals to digital values using the map() function.

## Instructions:
Building upon the concepts introduced in the previous activity, this exercise involves modifying the LED control logic while incorporating analog signal functionality. The following conditions should be implemented:

- Utilize pins 8 to 12 to connect the LEDs.
- Implement a running light pattern where LEDs turn on sequentially from pin 12 to 8 with a 1-second delay. After all LEDs are turned on, they should turn off in the same sequence, one by one.
- Use the analogWrite() function to control the brightness of each LED, demonstrating the use of pulse-width modulation (PWM) for analog signal simulation.
- Implement the logic using a while() loop and an array to define pin configurations dynamically.
