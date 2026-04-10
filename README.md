# Automatic Solar Tracking Drying System for Agricultural Products

A microcontroller-based automatic solar tracking drying system designed to improve drying efficiency for agricultural products by dynamically aligning the drying platform toward maximum sunlight.

The system uses dual LDR sensors placed in the front and back to detect light intensity. A threshold-based comparison algorithm determines the direction of maximum illumination, and the drying platform moves accordingly using a differential drive mechanism.

This project resulted in a published patent in sustainable agricultural technology.

---

## Key Features

- Automatic solar tracking
- Dual LDR light sensing
- Threshold-based decision logic
- Differential drive motion
- Two rear motor drive system
- Front castor wheel stabilization
- Microcontroller-based control
- Energy-efficient agricultural drying
- Patent published system

---

## System Architecture

Sensor Layer  
Two LDR sensors placed at front and back measure sunlight intensity.

Processing Layer  
Microcontroller compares sensor values and computes difference.

Control Layer  
Motor driver controls two rear motors.

Mechanical Layer  
Front castor wheel enables smooth directional movement.

---

## Working Principle

The system reads two LDR values:

Front LDR  
Back LDR  

The microcontroller computes:

difference = front − back

If:

|difference| < threshold → Stop  
difference > threshold → Move forward  
difference < −threshold → Move backward  

The drying platform moves toward the direction with maximum sunlight.

---

## Mechanical Design

Front: Castor wheel (free rotation)  
Rear: Two DC motors (differential drive)  

This allows the platform to move forward/backward to align with sunlight.

---

## Hardware Components

Microcontroller  
LDR Sensor (Front)  
LDR Sensor (Back)  
Motor Driver Module  
Two DC Motors  
Castor Wheel  
Drying Platform  
Power Supply  

---

## Applications

Solar agricultural drying  
Food dehydration systems  
Solar-based crop preservation  
Low-cost agritech drying systems  

---

## Achievement

Published Patent  
Automatic Solar Tracking Drying System for Agricultural Products

---

## Author

Noel Varghese George  
Embedded Systems | Hardware | Agritech | VLSI (Learning)

LinkedIn: https://linkedin.com/in/noel-varghese-george-a44333328  
GitHub: https://github.com/Noel01042006
