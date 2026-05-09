\# Discontinuous Conduction Mode (DCM)



\## DCM Definition



Discontinuous conduction mode (DCM) occurs when the inductor current reaches zero and remains at zero for a finite interval during the switching cycle.



In this operating mode:

\- the inductor fully releases its stored energy before the next switching cycle begins,

\- current conduction becomes discontinuous,

\- and converter behavior differs from continuous conduction mode.



\---



\## DCM by Inductance Reduction



The converter was forced into discontinuous conduction mode by reducing the inductance below the critical inductance value.



Simulation parameters:

\- L = 40 µH

\- R = 2.33 Ω

\- fs = 10 kHz



The reduced inductance increased current ripple significantly, causing the inductor current to reach zero before the next switching interval.



The resulting waveform clearly demonstrates:

\- discontinuous current behavior,

\- and a zero-current interval within each switching cycle.



Figure:

\- `IL\_DCM\_InductorReduction.png`



\---



\## DCM by Load Resistance Variation



Discontinuous conduction mode was also achieved by increasing the load resistance while maintaining the original inductance value.



Simulation parameters:

\- L = 103.25 µH

\- R = 5 Ω

\- fs = 10 kHz



Increasing the load resistance reduced the output current demand, causing the inductor current to decay to zero during the switching cycle.



This demonstrates that:

\- lighter load conditions can force the converter into DCM operation even without changing inductance.



Figure:

\- `IL\_DCM\_LoadVariation.png`



\---



\## DCM Characteristics



The obtained DCM waveforms demonstrate several important characteristics:



\- larger inductor current ripple,

\- discontinuous energy transfer,

\- increased current peaks,

\- zero-current intervals,

\- and stronger dependence on operating conditions.



Compared with CCM operation, DCM produces less stable current behavior and greater waveform variation.



\---



\## CCM versus DCM Behavior



Compared with CCM:

\- DCM operation produces higher ripple,

\- lower average inductor current,

\- and discontinuous current conduction.



The transition from CCM to DCM was successfully demonstrated using:

\- inductance reduction,

\- and load resistance variation.

