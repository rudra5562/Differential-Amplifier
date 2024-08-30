# Differential-Amplifier
### 1. **Circuit Setup:**
   - **Differential Pair (M1, M2):** Use two NMOS transistors as the input stage. Ensure proper sizing to meet the gain and bandwidth specifications.
   - **Active Load (M3, M4):** Implement the active load using PMOS transistors in a current mirror configuration.
   - **Tail Current Source (M0):** Use an NMOS transistor to set the bias current for the differential pair. This will also influence the common-mode rejection ratio (CMRR).
   - **Potential Division:** Use resistor dividers or voltage sources to set the bias points for the gates of M1, M2, and the active load. Ensure that all transistors operate in the saturation region.

### 2. **Biasing:**
   - Calculate the required bias current using the tail current source (M0) to achieve the desired slew rate and gain. Use the potential division method to set the gate voltages of M1 and M2.
   - Adjust the sizes of M3 and M4 to set the proper current mirror ratio for the desired gain.

### 3. **DC Analysis:**
   - Perform a DC operating point analysis to verify that all transistors are in the saturation region.
   - Check the bias voltages and currents to ensure they are within the expected range.

### 4. **AC Analysis:**
   - Conduct an AC sweep to determine the gain and bandwidth of the amplifier.
   - Adjust the widths (W) and lengths (L) of M1, M2, M3, and M4 to achieve a gain of 40 dB and a gain-bandwidth product (GBW) of 5 MHz.

### 5. **Transient Analysis:**
   - Perform a transient analysis to measure the slew rate. Apply a step input and observe the output waveform.
   - Adjust the tail current and load capacitance to meet the slew rate specification of 5 V/μs.

### 6. **Fine-Tuning:**
   - Iterate the design by adjusting transistor sizes, bias currents, and load capacitance based on the simulation results.
   - Ensure all performance metrics are met, and verify that the transistors remain in saturation during operation.

### 7. **Verification:**
   - Re-run the DC, AC, and transient analyses to confirm that the design meets the specified gain, slew rate, and GBW.
   - Document the final transistor sizes, bias currents, and operating points.

