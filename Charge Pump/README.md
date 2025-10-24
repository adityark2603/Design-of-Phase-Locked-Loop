# Charge Pump
The Charge Pump (CP) is a key analog component in a Charge-Pump Phase-Locked Loop (CP-PLL) that interfaces the digital output of the Phase Frequency Detector (PFD) to the analog input of the Voltage Controlled Oscillator (VCO). It effectively converts the PFD's UP and DOWN digital error pulses into an analog current, which is then fed to the Loop Filter (LF) to generate the smooth control voltage for the VCO.

### <ins>Key Features:</ins>
- **Digital-to-Analog Conversion**: The CP is a current-steering circuit that uses the PFD's UP/DOWN signals to selectively pump a fixed current ($I_{CP}$) into or sink it out of the loop filter capacitor.
- **Current Mismatch Mitigation**: In CMOS CPs, current mismatch between the charge (UP) and discharge (DOWN) currents can cause ripple and static phase error. Advanced designs, often necessary in advanced nodes like 45nm and below, employ techniques like gain-boosting or current mirrors to ensure precise current matching.
- **Low Noise and Jitter**: The CP's output current ripple, which is converted to a voltage ripple by the Loop Filter, directly contributes to the output phase noise and jitter of the PLL. Minimizing this current ripple is critical for high-performance applications.

