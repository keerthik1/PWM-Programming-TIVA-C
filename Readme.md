# Varying LED Intensity Using PWM on TIVA C LaunchPad

## Overview
This project demonstrates varying the intensity of an LED using Pulse Width Modulation (PWM) on the TIVA C LaunchPad (EK-TM4C123GXL, TM4C123GH6PM microcontroller). The onboard RGB LED (e.g., PF3 for Green) is controlled by adjusting the PWM duty cycle, allowing smooth brightness transitions. The project showcases embedded systems skills, including PWM configuration, timer setup, and GPIO control, with applications in lighting control and user feedback systems.

### Features
- Controls LED brightness by varying the PWM duty cycle (0% to 100%).
- Uses the TIVA C LaunchPad’s onboard RGB LED (PF3, green) for demonstration.
- Implements a fading effect by incrementally adjusting the duty cycle.
- Configures the system clock to 16 MHz for precise PWM timing.
- Supports manual duty cycle adjustment via code modification.

## Hardware Requirements
- **TIVA C LaunchPad**: EK-TM4C123GXL with TM4C123GH6PM microcontroller.
- **LED**: Onboard RGB LED (PF2 for blue; alternatively, PF1 for red or PF3 for green).
- **Optional External LED**: If using an external LED, connect it to a PWM-capable pin (e.g., PF2) with a current-limiting resistor (e.g., 330 ohms).
- **Connections** (if using external LED):
  - LED Anode → PF3 (PWM pin)
  - LED Cathode → GND (via resistor)
  - Note: The onboard LED is already connected and can be used directly.

## Software Requirements
- **Code Composer Studio (CCS)**: Version 12.4.0 or later.
- **TivaWare**: Optional (this project uses direct register access for educational purposes).
- **Compiler**: TI ARM Compiler (included with CCS).

## Setup Instructions
1. **Hardware Setup**:
   - If using the onboard LED, no additional connections are needed.
   - If using an external LED, connect it to PF3 (or another PWM-capable pin) as described above.
   - Power the LaunchPad via USB.
2. **Software Setup**:
   - Clone or download this repository.
