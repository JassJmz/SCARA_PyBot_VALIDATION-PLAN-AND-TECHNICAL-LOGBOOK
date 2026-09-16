# Technical Logbook — SCARA_PyBot

Running log of project progress. Add a new dated entry each work session; do not edit past entries.

---

## Entry 1 — September 14, 2026

**Team members:**
- Jassiel Obed Jiménez Ochoa
- Tania Elizabeth Serrano Hernandez
- Bryan Emmanuel Barboza Carrillo
- Eber Jafet Rodriguez Valenciano

**Current project status:** Phase 1 (system architecture, main components, HW/SW partition
and preliminary BOM, U1A4) is complete. Phase 2 (validation planning) is in progress: KPIs,
validation table and test cases defined.

**Work completed:**
- Reviewed the U1A4 architecture, block diagram and BOM as the baseline for validation.
- Selected 5 KPIs relevant to the SCARA arm (positioning accuracy, repeatability, power
  consumption, Wi-Fi latency, step-pulse stability).
- Built the validation table with instruments, procedures, expected values and acceptance
  criteria.
- Defined 4 reproducible test cases covering homing, accuracy, power and communication
  safety.
- Created the project repository skeleton (`hardware/`, `firmware/`, `documentation/`,
  `tests/`, `README.md`).

**Problems found:**
- No oscilloscope/logic analyzer has been reserved yet for the STEP-pulse and Wi-Fi latency
  tests (TC4 and the step-rate KPI); needs to be scheduled with the lab.
- The A4988/ESP32-S3 lead-time risk identified in U1A4 still stands — components have not
  been ordered yet, which could delay the first physical test run.

**Decisions made:**
- Positioning accuracy was chosen as the primary KPI, since it most directly reflects the
  pick-and-place purpose of the arm.
- Homing repeatability will be validated before absolute positioning accuracy, since the
  zero reference must be trustworthy first.
- A simple caliper-and-grid method was chosen over a vision-based measurement system for the
  first validation pass, to keep the test setup low-cost and fast to execute.

**Next task:** Order the BOM components, set up the ESP32-S3 firmware environment
(FastAccelStepper bench test per U1A4 risk #5), and run Test Case 1 (homing repeatability)
as soon as the mechanical assembly and at least one axis are wired.

---

## Entry 2 — [date]

**Team members:**

**Current project status:**

**Work completed:**

**Problems found:**

**Decisions made:**

**Next task:**
