\# Continuous Conduction Mode (CCM) Operation



\## CCM Definition



Continuous Conduction Mode (CCM) occurs when the inductor current never reaches zero during the switching cycle.



In this operating mode:

\- the inductor continuously stores and releases energy,

\- the output voltage ripple remains relatively small,

\- and the converter operates with stable energy transfer characteristics.



\---



\## CCM Simulation Objective



The converter was simulated in CCM to verify:

\- proper buck converter operation,

\- output voltage regulation near 7 V,

\- acceptable output voltage ripple,

\- and continuous inductor current behavior.



\---



\## Simulation Parameters



| Parameter | Value |

|---|---|

| Input Voltage | 24 V |

| Output Voltage | 7 V |

| Output Current | 3 A |

| Switching Frequency | 10 kHz |

| Duty Cycle | 29.2 % |

| Inductance | 103.25 µH |

| Capacitance | 857.14 µF |

| Load Resistance | 2.33 Ω |



\---



\## Output Voltage Behavior



The output voltage waveform demonstrates successful buck converter operation.



The converter reduces the input voltage from 24 V to approximately 7 V while maintaining relatively small ripple around the average output value.



The steady-state ripple voltage remained within the design target.



Figure:

\- `Vo\_CCM\_SteadyState.png`



\---



\## Input and Output Voltage Comparison



The comparison between input and output voltages clearly demonstrates the voltage step-down behavior of the buck converter.



Figure:

\- `Vin\_vs\_Vo\_CCM.png`



\---



\## PWM Switching Signal



The PWM waveform verifies:

\- fixed-frequency switching operation,

\- correct duty cycle implementation,

\- and proper MOSFET gate control.



Figure:

\- `PWM\_10kHz\_29p2.png`



\---



\## MOSFET Switching Voltage



The MOSFET drain-source voltage waveform demonstrates proper switching operation between ON and OFF states.



Figure:

\- `MOSFET\_VDS\_CCM.png`



\---



\## Inductor Current Analysis



The inductor current waveform confirms continuous conduction mode operation.



The current waveform:

\- exhibits triangular ripple behavior,

\- remains continuous during the switching cycle,

\- and never reaches zero.



This behavior verifies successful CCM operation.



Figure:

\- `IL\_CCM.png`



\---



\## Output Voltage Ripple Verification



The steady-state output voltage ripple was measured from the simulated waveform.



Measured ripple values:



| Parameter | Value |

|---|---|

| Maximum Output Voltage | ≈ 7.13 V |

| Minimum Output Voltage | ≈ 7.07 V |

| Ripple Voltage | ≈ 0.06 V |



The measured ripple voltage is significantly smaller than the assignment allowable limit of 0.5 V.



This confirms:

\- proper capacitor sizing,

\- stable converter operation,

\- and successful output filtering performance.



\---



\## CCM Verification Summary



The simulated converter successfully achieved continuous conduction mode operation.



The obtained results verified:

\- correct voltage step-down behavior,

\- stable PWM switching operation,

\- continuous inductor current,

\- and acceptable output voltage ripple.



The converter therefore satisfies the required CCM operating conditions.

