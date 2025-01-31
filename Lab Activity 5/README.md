## Laboratory Activity #5

## Objectives:
- Understand and implement Arduino Serial Communication.
- Utilize Python as a tool for handling serial connections.
- Develop a system where an Arduino circuit can be controlled using Python and FastAPI via HTTP requests.
## Prerequisites:
To complete this activity, ensure the following are available and installed.

## Hardware:
- Arduino board
- USB cable for connection

## Software:
- Arduino IDE
- Python (version 3.x)

## Description:
- This project establishes a serial communication interface between an Arduino board and a FastAPI backend, allowing an LED to be controlled remotely via HTTP requests. The FastAPI server acts as a bridge, sending commands through a serial connection, enabling users to turn the LED on and off using API endpoints.

## Implementation Steps:
- Set up the circuit according to the diagram in A5-Diagram.png.
- Upload the Arduino code using the Arduino IDE, ensuring the correct serial port is selected.
- Create a Python script to send commands to the Arduino via the serial port.
- Integrate Arduino control into a web API using FastAPI.

## Running the Server:
- To start the FastAPI server, use the following command: fastapi dev <name_of_file>.py

## Testing the API via Command Line:
- Turn LED On: curl -X POST http://127.0.0.1:8000/led/on
- Turn LED off:curl -X POST http://127.0.0.1:8000/led/off

## Key Concepts in the Python Code:
- Serial Initialization: Establishes a serial connection with the Arduino using COM5 and a 9600 baud rate.
- Delay (2 seconds): Ensures the Arduino completes its reset and initialization.
- Write Commands: Sends "1" to turn the LED on and "0" to turn it off via the serial interface.

## Additional Notes:
- This activity can be extended to Laboratory Activity 6, where another Arduino setup will control this LED system remotely.
- This project demonstrates the integration of embedded systems with web technologies, providing a foundation for IoT applications.
