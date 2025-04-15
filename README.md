# Closed Loop BLDC Motor Drive

![image](https://github.com/user-attachments/assets/70774e97-5498-40fa-bbe2-e15c952afa01)


## Overview

This repository contains the MATLAB Simulink model for a BLDC motor-driven in closed loop. The model is designed to simulate and analyze the performance of a BLDC motor using an inverter-based electronic commutation system with Hall sensor feedback. A PID-based closed-loop speed controller is implemented to ensure precise speed regulation.

## Features

- **BLDC Motor Simulation**: Implements a brushless DC motor model with trapezoidal back EMF.
- **Inverter-Based Commutation**: Uses a three-phase inverter to drive the motor.
- **Hall Sensor Feedback**: Determines rotor position for proper phase commutation.
- **PID Speed Control**: Ensures accurate speed regulation.

## System Components

1. **BLDC Motor Model**: Simulated using Simulink’s Permanent Magnet Synchronous Motor block (Trapezoidal Back EMF).
2. **Three-Phase Inverter**: Converts DC input into three-phase AC output to drive the motor.
3. **Hall Sensor Logic**: Determines the correct switching sequence.
4. **PID Controller**: Regulates motor speed based on the reference input.

## Installation & Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/bldc-bicycle.git
   ```
2. Open MATLAB and navigate to the project directory.
3. Open the Simulink model (`bldc_bicycle.slx`).
4. Run the simulation and observe motor behavior.

## Current Status

The simulation is not yet complete. The PID controller parameters still need to be properly tuned to achieve the desired speed control performance.

## License

This project is licensed under the **MIT License**. See the LICENSE file for details.

## Contact

For any queries, feel free to reach out or raise an issue in the repository.

🚴⚡ Happy Simulating!

