# firmware/

ESP32-S3 firmware for SCARA_PyBot (planned modules, not yet implemented):

- `kinematics/` — forward/inverse kinematics, point-to-point trajectory interpolation
- `motion/` — STEP/DIR pulse generation and acceleration ramps (e.g., FastAccelStepper)
- `homing/` — limit-switch reading, debouncing, homing sequence
- `gripper/` — PWM control for the SG90 servo
- `comm/` — Wi-Fi command API / web server, USB-UART debug interface
- `safety/` — soft limits, watchdog, connection-loss timeout stop

First bench test to run here: validate the step-generation library on the ESP32-S3
dual-core/timer peripherals (see U1A4 technical risk #5) before wiring it into the full
control loop.
