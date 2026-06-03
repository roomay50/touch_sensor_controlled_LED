# **Touch Sensor Controlled LED Sequence (Arduino Uno)**
## **Overview**

This project demonstrates how an Arduino Uno can be used to control a sequence of three LEDs using a touch sensor input. Each tap on the sensor triggers a change in state, cycling through the LEDs one after another.

The system reads a digital input from the sensor and uses a counter-based switch logic to determine which LED should be activated.

## **How It Works**

A touch sensor is connected as a digital input to the Arduino Uno
Each touch is detected as a HIGH signal
The Arduino increments a counter on every valid touch
A switch case structure is used to control LED states:
First touch → LED 1 ON
Second touch → LED 2 ON
Third touch → LED 3 ON

After the third LED, the cycle can be reset depending on the code logic.

## **Hardware Setup**
- Arduino Uno
- Touch sensor module (capacitive sensor used in actual implementation)
- 3 LEDs
- Resistors (330Ω recommended)
- Breadboard and jumper wires

## **Important Note on Simulation vs Real Hardware**

The Tinkercad simulation uses a push button because a capacitive touch sensor is not available in the simulator.

Simulation (Push Button): Configured with INPUT_PULLUP, so the input reads LOW when the button is pressed.
Hardware (Touch Sensor): The capacitive touch sensor outputs HIGH when touched.

If you are building the physical circuit, replace the push button in the schematic with a capacitive touch sensor and update the input condition in the code accordingly.



## **Project Files**
- sensor_as_input.ino → Arduino source code
- Circuit diagram (button-based simulation)
- Demo video (touch sensor hardware implementation)

## **Learning Outcomes**
- Reading digital input signals in Arduino
- Using state-based logic with counters
- Implementing switch case control flow
- Understanding real hardware vs simulation differences

