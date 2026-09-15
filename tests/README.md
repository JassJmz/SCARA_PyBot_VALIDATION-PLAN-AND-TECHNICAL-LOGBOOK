# tests/

Test case records and captured results for SCARA_PyBot. Full definitions of each test case
are in `documentation/Validation_Plan_SCARA.pdf`; this folder holds the raw evidence once
each test is actually run:

- `TC1_homing_repeatability/` — 10-run position measurements, computed std. dev.
- `TC2_positioning_accuracy/` — measured deviation at each of the 5 reference points
- `TC3_power_draw/` — current logs during idle and full 3-axis load
- `TC4_wifi_latency/` — latency samples and connection-loss safety-stop timing

No results recorded yet — components have not been ordered (see the technical logbook).
