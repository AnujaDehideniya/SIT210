Project Overview

This repository contains the Arduino code for a smart lighting system designed to help Linda safely enter her home during winter evenings. When a push button is pressed:

Porch light turns ON for 30 seconds
Hallway light turns ON for 60 seconds

The system uses modular programming to manage light activation and timing efficiently without blocking the main loop.

Code Structure

The Arduino code is organized into three main modules:

handleSwitch() – Detects when the push button is pressed and triggers the lights.
startLights() – Turns both porch and hallway LEDs ON and records the start time for timing.
updateLights() – Monitors elapsed time and turns off each light automatically when its duration ends.

This modular approach makes the code readable, maintainable, and scalable, allowing easy addition of new lights or sensors in the future.

How to Use
Connect the porch LED to Arduino pin D2 and the hallway LED to D3.
Connect a push button to pin D4 and GND.
Upload the code to an Arduino Nano 33 IoT.
Press the button to turn on the lights.
Porch light turns off after 30 seconds.
Hallway light turns off after 60 seconds.
Hardware Components
Arduino Nano 33 IoT
2 LEDs 
2 resistors 
Push button
Breadboard & jumper wires
