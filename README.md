# SCARA_PyBot

Embedded control system for a SCARA-type robotic arm (JJRobots PyBot platform), built for
educational pick-and-place tasks. Developed as the term project for *Sistemas Embebidos*
(9th semester, ITSRLL).

## What it does

An ESP32-S3-DevKitC-1 drives three joints (shoulder, elbow, and a linear Z axis) through
A4988 stepper drivers and NEMA17 motors, homes each axis against a mechanical limit switch
on power-up, and actuates an SG90 servo gripper as the end effector. The arm can be
controlled locally over USB/UART or remotely over Wi-Fi.

See [`documentation/Report_Phase1_SCARA.docx`](documentation/Report_Phase1_SCARA.docx) for
the full system architecture, block diagram, HW/SW partition and BOM (U1A4), and
[`documentation/Validation_Plan_SCARA.pdf`](documentation/Validation_Plan_SCARA.pdf) for the
KPI validation plan, test cases and technical logbook (U1A5).

## Repository structure

```
SCARA_PyBot/
├── hardware/        BOM, block diagram, wiring references
├── firmware/        ESP32-S3 source code (kinematics, motion control, homing, Wi-Fi API)
├── documentation/   Architecture report, validation plan, technical logbook
├── tests/           Test case records and captured results
└── README.md
```

## Status

Phase 1 (system architecture and HW/SW partition) is complete. Phase 2 (validation
planning) is in progress — see the technical logbook in
[`documentation/Technical_Logbook.md`](documentation/Technical_Logbook.md) for the latest entry.

## Team

Jassiel Obed Jiménez Ochoa — update this section with teammates if the project is
completed as a team of up to 4 students.
