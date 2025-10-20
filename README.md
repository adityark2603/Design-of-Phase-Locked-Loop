# Design-of-Phase-Locked-Loop
### <ins> Block Diagram of PLL Architecture: </ins>

<img width="606" height="228" alt="image" src="https://github.com/user-attachments/assets/eb2baad3-ae12-44b9-a6c5-a3b4b14a107b" />

#### <ins>NOTE:</ins> 
To build the complete PLL architecture, I used some standard gates, such as `AND`, `NOR`, and `NOT`. <br>
I also used two types of D Flip-Flops: `DFF_Reset` and `TSPC DFF`. <br>
Reference: [Prerequisite Standard Gates & Circuits](https://github.com/adityark2603/Design-of-Phase-Locked-Loop/tree/main/Prerequisite%20Standard%20Gates%20%26%20Circuits)

### <ins> Role of PFD in PLL: </ins>
1. The PFD operates by receiving two input signals (reference and divider outputs), and its output transitions help detect both phase and frequency differences.​
2. Digital D-type flip-flops (DFFs) are used in a typical PFD implementation, for robust operation under low voltage (1.0–1.2V) and high-speed switching in the 45nm process node.
