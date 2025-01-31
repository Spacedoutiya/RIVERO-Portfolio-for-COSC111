## Lab Activity #3

## Objectives:
- Introduce the fundamental sensor components commonly used in Internet of Things (IoT) applications.
- Integrate sensor components into an Arduino-based circuit.
- Develop a basic fire detection system using a thermistor and a photoresistor.

## Description:
- This activity focuses on building a simple fire detection system using an Arduino Uno. The system utilizes a thermistor to measure temperature and a photoresistor to detect light intensity. If both the temperature and brightness exceed predefined thresholds, a fast-blinking red LED serves as a fire warning indicator. This hands-on project helps students understand the integration of analog sensors, digital signals, and conditional programming in Arduino-based systems.

## Instructions:
- Construct a Fire Sensor System utilizing a thermistor and a photoresistor to detect fire-related conditions.

## Implementation Details:
- Connect the thermistor to analog pin A0 and the photoresistor to analog pin A2.
- Measure temperature in Celsius and process the photoresistor as a digital signal for brightness detection.
  
## Define the threshold values as:
- Temperature: 50°C or higher
- Brightness Level: 220 or higher
- If both thresholds are exceeded, trigger a fast-blinking red LED connected to digital pin 12 as a fire alert.
