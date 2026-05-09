\# System Architecture



\## Open-Loop Buck Converter Overview



The implemented system is an open-loop DC-DC buck converter designed to reduce a 24 V DC input voltage to approximately 7 V DC output voltage.



The converter was implemented using Simscape Electrical Specialized Power Systems in MATLAB/Simulink under discrete-time simulation conditions.



The converter operates using pulse-width modulation (PWM) switching control with a fixed duty cycle.



\---



\## Main Power Stage Components



The converter consists of the following main components:



\### DC Voltage Source

Provides the input supply voltage of 24 V.



\### MOSFET Switch

Acts as the main high-speed switching device controlled using a PWM pulse generator.



\### Freewheeling Diode

Provides an alternate current path during the MOSFET OFF interval to maintain continuous inductor current flow.



\### Inductor

Stores energy during the ON state and releases energy during the OFF state to smooth current variations.



\### Capacitor

Reduces output voltage ripple and stabilizes the output voltage waveform.



\### Resistive Load

Represents the output power consumption corresponding to the required output current.



\---



\## PWM Control System



The converter uses an open-loop PWM control strategy.



The PWM pulse generator parameters were configured as:



| Parameter | Value |

|---|---|

| Switching Frequency | 10 kHz |

| Duty Cycle | 29.2 % |

| Pulse Amplitude | 10 V |



The duty cycle was selected according to the ideal buck converter relationship:



D = Vo / Vin



\---



\## Simulation Environment



The simulation was performed using:

\- discrete solver configuration,

\- powergui block,

\- sampling time of 10e-6 sec.



The selected switching frequency satisfies the assignment simulation constraints while maintaining acceptable waveform resolution.



\---



\## System Architecture Figures



\### Complete Simulink Architecture



Figure: `buck\_converter\_final\_architecture.png`



\### PWM and Discrete Simulation Configuration



Figures:

\- `PWM\_10kHz\_29p2.png`

\- `powergui\_discrete\_settings.png`



\### Measurement and Monitoring Architecture



Figure:

\- `measurement\_architecture\_v1.png`

