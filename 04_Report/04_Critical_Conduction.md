\# Critical Conduction Mode



\## Critical Conduction Definition



Critical conduction mode represents the boundary between continuous conduction mode (CCM) and discontinuous conduction mode (DCM).



At this operating condition:

\- the inductor current decreases to approximately zero at the end of each switching cycle,

\- but does not remain at zero for a significant interval.



This operating point is also known as:

\- boundary conduction mode (BCM).



\---



\## Critical Inductance



The critical inductance separating CCM and DCM operation is given by:



Lcrit = ((1 - D)R) / (2fs)



Using:

\- D = 0.292

\- R = 2.33 Ω

\- fs = 10 kHz



the calculated critical inductance is approximately:



Lcrit ≈ 82.6 µH



\---



\## Critical Conduction by Inductance Reduction



The converter inductance was reduced from:



\- 103.25 µH

to:

\- 82.6 µH



while maintaining:

\- constant switching frequency,

\- constant duty cycle,

\- constant load resistance.



The resulting inductor current waveform approached zero at the end of the switching cycle, indicating operation near the CCM/DCM boundary.



Figure:

\- `IL\_Critical\_Mode.png`



\---



\## Critical Conduction by Load Variation



The converter was also driven toward critical conduction by increasing the load resistance while maintaining the original inductance value.



Simulation parameters:

\- L = 103.25 µH

\- R = 4 Ω



The reduced load current caused the inductor current minimum value to approach zero.



This demonstrates that converter operating mode depends on both:

\- inductance,

\- and load resistance.



Figure:

\- `IL\_Critical\_LoadVariation.png`



\---



\## Critical Mode Characteristics



The obtained waveforms demonstrate several important characteristics of critical conduction operation:



\- increased inductor current ripple,

\- reduced stored magnetic energy,

\- operation close to discontinuous conduction,

\- and increased sensitivity to parameter variations.



Critical conduction mode represents the transition region between stable CCM operation and fully discontinuous current behavior.

