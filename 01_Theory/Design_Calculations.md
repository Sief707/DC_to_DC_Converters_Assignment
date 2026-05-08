\# Buck Converter Design Calculations



\## Given Specifications



\- Input Voltage = 24 V

\- Output Voltage = 7 V

\- Output Current = 3 A



\## Design Assumptions



\- Ideal buck converter operation

\- Continuous conduction mode (CCM)

\- Switching frequency selected as 20 kHz

\- Output voltage ripple kept below 0.5 V as required

\- Inductor ripple current selected later as percentage of load current



\## Output Power



Po = Vo × Io



Po = 21 W



\## Load Resistance



R = Vo / Io



R = 2.33 Ω



\## Duty Cycle



D = Vo / Vin



D = 0.292



Duty cycle is approximately 29.2%.



\## Inductor Ripple Current Selection



The inductor ripple current was selected as 30% of the rated load current.



ΔIL = 0.3 × Io



ΔIL = 0.9 A



This value provides visible ripple while maintaining stable CCM operation.



\## Inductor Design



The inductor value for the buck converter is calculated using:



L = ((Vin - Vo) × D) / (ΔIL × fs)



Calculated inductance:



L ≈ 276 µH



A practical standard value of 300 µH was selected.



\## Output Voltage Ripple Selection



The assignment allows output voltage ripple less than 0.5 V.



A smaller ripple target of 0.1 V was selected to improve output quality and waveform smoothness.



\## Capacitor Design



The output capacitor is calculated using:



C = ΔIL / (8 × fs × ΔVo)



Calculated capacitor value:



C ≈ 56 µF



A practical value of 100 µF was selected.



\## Critical Inductance



The critical inductance separating CCM and DCM is calculated as:



Lcrit = ((1 - D) × R) / (2 × fs)



Lcrit ≈ 41 µH



Since the designed inductance is significantly larger than the critical inductance, the converter operates in continuous conduction mode.

