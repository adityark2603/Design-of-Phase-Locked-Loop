# Phase Locked Loop
### **<ins>Locking Behavior</ins>**

From the transient waveform, the control voltage (Vc) initially varies and gradually stabilizes. This indicates the PLL acquiring lock, as the VCO frequency adjusts until its output phase aligns with the reference input ($V_{ref}$).

→ The loop settles after the transient period (~1.0 µs).

### **<ins>Frequency Synchronization</ins>**

The VCO output (Vout) waveform (orange trace) initially has a changing frequency, but after lock, it becomes steady and matches the reference frequency when divided by the feedback divider.

→ Confirms that the PLL successfully maintains frequency synchronization between $V_{ref}$ and $V_{div}$.

### **<ins>PFD and Charge Pump Activity</ins>**

The UP and DOWN signals (from the PFD) show alternating pulses during the unlocking phase. Once the loop locks, these pulses become narrow and infrequent, showing minimal phase error.

→ Indicates proper operation of the PFD–Charge Pump–Loop Filter control path.
