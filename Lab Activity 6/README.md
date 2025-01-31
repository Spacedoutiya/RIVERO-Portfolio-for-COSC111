## Objectives:
- Develop a system that detects button presses using an Arduino and transmits the button state to a Python script.
- Implement API-based control, where the Python script triggers an HTTP request based on the button press.
- Establish a wireless connection (Wi-Fi or hotspot) between devices for remote communication.

## Prerequisites:
Ensure the following hardware and software are available and installed.

## Hardware:
- Arduino board
- USB cable for Arduino connection

## Software:
- Arduino IDE
 Python (version 3.x) with the required libraries: pip install pyserial requests fastapi[standard]

## Description:
- This project focuses on button press detection using an Arduino, which then communicates the button state to a Python script via serial communication. The script subsequently triggers an API request to another device connected via Wi-Fi or a hotspot. This second device has its own Arduino and LED setup, which responds to the received API commands.

## Implementation Steps:
- Set up the circuit based on the provided A6-Diagram.png.
- Upload the .ino code to the Arduino using the Arduino IDE, ensuring the correct serial port is selected.
- Modify the Python script to reflect your local IP address, ensuring it correctly communicates with the Arduino via serial connection.
- Integrate API control using FastAPI, allowing button presses to trigger LED state changes on a remote device.
- Use the requests library to send HTTP requests when the button is pressed.

## Running the Server:
- To start the FastAPI server, execute:fastapi dev <name_of_file>.py

## Testing the API via Command Line:
- Turn LED On: curl -X POST http://127.0.0.1:8000/led/on
- Turn LED Off: curl -X POST http://127.0.0.1:8000/led/off

## Key Concepts in the Python Code:
- Button Press Detection: The Arduino continuously monitors the button state and sends updates over serial communication.
- Serial Communication: The Python script reads the serial input from the Arduino.
- API Call Trigger: When the button is pressed, the script sends an HTTP request to control the LED on the second Arduino.
- Network Communication: The system relies on Wi-Fi or a hotspot to communicate between the two devices.

## Additional Notes:
- This activity is linked to Laboratory Activity 5, where the remote LED setup is controlled by this Arduino button system.
- This project demonstrates the integration of embedded systems with web technologies, enabling remote IoT device control.

