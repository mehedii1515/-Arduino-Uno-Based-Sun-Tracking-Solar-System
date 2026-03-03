Arduino Uno Based Sun Tracking Solar System
This project presents an innovative approach to enhance solar energy harvesting efficiency by implementing a sun-tracking mechanism using an Arduino Uno. By dynamically aligning solar panels with the sun's trajectory, the system maximizes energy yield throughout the day.

Project Overview
The Arduino Uno Based Sun Tracking Solar System optimizes solar panel orientation to ensure they continuously face the sun for maximum exposure. It integrates light sensors and servo motors to detect sunlight direction and control panel positioning in real-time. This provides a cost-effective solution for sustainable energy, particularly in locations with varying sunlight angles.

Key Features

Dynamic Alignment: Automatically aligns panels with the sun's trajectory to optimize efficiency.


Real-time Processing: Uses the Arduino Uno’s computational power for precise motor control based on sensor inputs.


Increased Energy Yield: Extends the window of use and increases output even in variable weather.


IoT & Renewable Integration: Showcases the potential of combining electronics with renewable energy systems.

Equipment (Parts & Tools)
Components

Microcontroller: Arduino Uno R3.


Solar Panels: 5V 1 Watt (3 pcs).


Sensors: LDR Sensors (2 pcs).


Actuator: Mini Servo Motor SG90.

Power Management:

LiPo Battery Charger Module TP4056.

3.7V Battery Cell (Model 18650).

USB DC 1~5V to DC 5V Step Up Boost Module.


Other: 100k Resistors, Power Switch, Jumper Wires, and 5mm Wood Panel.

How It Works

Light Sensing: Two LDR sensors are placed on the horizontal sides of the solar panel.


Comparison: The Arduino reads the analog values from both sensors, LDR1 and LDR2.


Tolerance: A set tolerance of 20 prevents constant, jittery motion if the light values are nearly identical.


Movement: If one sensor detects more light than the other, the Arduino signals the servo motor to rotate the panel eastward or westward.


Limits: The system is programmed to stay within a 0 to 180-degree range to prevent mechanical overextension.

Installation & Procedure

Framework: Cut a 60x60 cm wood panel and build a custom stand for horizontal movement.


Solar Connection: Solder the three solar panels in series to achieve a 5V 3-Watt supply.


Power Circuit: Connect the panels to the TP4056 charger and the 3.7V battery. Use the Step-Up Boost module to power the Arduino's 5V and GND ports.


Wiring: Attach LDRs with 100k resistors to the GND and 5V pins.


Code: Upload the source code to the Arduino Uno R3 to enable full tracking functionality.

Conclusion
This project demonstrates the potential of accessible automation in renewable energy. By utilizing innovative technology, we can build a greener, more efficient future for solar harvesting.
