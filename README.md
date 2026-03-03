# Arduino Uno Based Sun Tracking Solar System

An innovative approach to enhancing solar energy harvesting efficiency by implementing a sun-tracking mechanism using an Arduino Uno microcontroller. This system ensures solar panels continuously face the sun for maximum exposure, significantly increasing energy yield compared to stationary setups.

---

## Project Overview

The core objective of this project is to optimize solar panel orientation in real-time. By integrating light sensors and a servo motor, the system detects the direction of the strongest sunlight and adjusts the panel positioning accordingly. 

### Key Features
* **Dynamic Tracking**: Automatically aligns panels with the sun's trajectory throughout the day.
* **Precise Control**: Utilizes the Arduino Uno for real-time data processing and motor adjustment.
* **Cost-Effective**: Built using accessible components like LDRs and a standard SG90 servo motor.
* **Sustainable Design**: Focuses on maximizing renewable energy efficiency.

---

## Equipment & Components

### Hardware
* **Microcontroller**: Arduino Uno R3
* **Solar Panels**: 5V 1 Watt (3 units connected in series)
* **Sensors**: 2x LDR (Light Dependent Resistors)
* **Actuator**: Mini Servo Motor SG90
* **Power Management**:
    * TP4056 LiPo Battery Charger Module
    * 3.7V 18650 Battery Cell
    * 1~5V to 5V Step-Up Boost Module
* **Other**: 100k Resistors, Power Switch, 5mm Wood Panel (60x60cm frame)

### Tools Used
* Soldering Iron & Lead
* Glue Gun
* Wood/Wire Cutters

---

## How It Works



1. **Detection**: Two LDR sensors are mounted on the horizontal sides of the solar panel.
2. **Logic**: The Arduino compares the light values from both sensors. A "tolerance" variable is used to prevent the motor from jittering when light levels are nearly equal.
3. **Movement**: If one side receives more light, the Arduino signals the servo motor to rotate the panel in that direction (East or West).
4. **Safety**: The code includes limits to ensure the motor stays within a 0–180 degree range.

---

## Implementation Procedure

1. **Structural Build**: Construct a 60x60 cm frame with a custom stand to allow for horizontal movement.
2. **Power Setup**: Solder the solar panels in series. Connect them to the TP4056 charger and the 18650 battery. 
3. **Voltage Regulation**: Connect the Step-Up Boost module to provide a steady 5V to the Arduino from the battery.
4. **Wiring**: Connect LDRs with 100k resistors to the analog pins and ground. Attach the servo signal wire to digital pin 2.
5. **Firmware**: Upload the tracking logic to the Arduino via the IDE.

---

## Conclusion

This project showcases the potential of combining IoT technology with renewable energy. It provides a scalable, accessible solution for improving solar efficiency in residential or small-scale industrial applications.
