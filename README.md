# Design-of-Phase-Locked-Loop
### <ins> Block Diagram of PLL Architecture: </ins>

<img width="606" height="228" alt="image" src="https://github.com/user-attachments/assets/eb2baad3-ae12-44b9-a6c5-a3b4b14a107b" />

#### <ins>NOTE:</ins> 
To build the complete PLL architecture, we'll use some standard gates, such as `AND`, `NOR`, and `NOT`. <br>
We'll also use two types of D Flip-Flops: `DFF_Reset` and `TSPC DFF`. <br>
Refer Directory: [Prerequisite Standard Gates & Circuits](https://github.com/adityark2603/Design-of-Phase-Locked-Loop/tree/main/Prerequisite%20Standard%20Gates%20%26%20Circuits)

### <ins> Role of PFD in PLL: </ins>
1. The PFD operates by receiving two input signals (reference and divider outputs), and its output transitions help detect both phase and frequency differences.​
2. Digital D-type flip-flops (DFFs) are used in a typical PFD implementation, for robust operation under low voltage (1.0–1.2V) and high-speed switching in the 45nm process node.

### <ins> Role of CP in PLL: </ins>
1. It converts the digital phase/frequency error pulses from the detector into analog current pulses.
2. It pumps the error current into the loop filter, which integrates it to produce the smooth DC control voltage ($\boldsymbol{V}_{\mathbf{c}}$) that tunes the VCO frequency.

### <ins> Role of CSVCO in PLL:</ins>
1. The current-starved VCO’s oscillation frequency is controlled by the bias current, allowing precise tuning of the output frequency in response to the control voltage from the PLL.
2. It limits the current through the delay stages, reducing overall power consumption compared to a regular ring VCO.
3. Its design is compact and fully CMOS-compatible, making it ideal for on-chip PLL implementations.
