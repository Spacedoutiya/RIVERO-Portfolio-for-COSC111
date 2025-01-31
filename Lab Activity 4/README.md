## Lab Activity #4

## Objectives:
- Gain an understanding of Arduino Serial Communication and its implementation.
- Explore and utilize basic Serial connection functions for data exchange.
- Develop a sensor-based circuit that can be controlled via Serial communication.

#Description:
This activity focuses on using Serial communication to interact with an Arduino-based circuit. A sensor will be used to monitor either temperature (using a thermistor) or brightness (using a photoresistor). When the sensor's reading exceeds a predefined threshold, an LED connected to pin 13 will blink continuously, even if the sensor reading later drops below the threshold. The blinking can only be stopped by entering the command "stop" in the Serial Monitor, regardless of letter case. 

Instructions:
Using the circuit diagram and code structure from Laboratory Activity 3, complete the following tasks:

## Select one (1) sensor for this activity:

- Thermistor: Set the temperature threshold to 50°C.
- Photoresistor: Set the brightness threshold to 220.

## Implement the following logic:
- If the sensor reading exceeds the threshold, the LED on pin 13 should start blinking with a 100ms delay between ON and OFF states.
- The blinking must continue even after the sensor reading drops below the threshold.

## Serial Communication Control:

- If the user enters the word "stop" in the Serial Monitor, the LED should stop blinking.
- The input should be case-insensitive, meaning commands such as "STOP," "Stop," or "sToP" should all work.

## Evaluation Criteria:
The circuit and code must successfully detect threshold breaches and trigger persistent LED blinking.
The blinking should not stop unless the "stop" command is entered via Serial Monitor.
Proper use of Serial communication functions in the code.
Implementation of case-insensitive string comparison for user input.
