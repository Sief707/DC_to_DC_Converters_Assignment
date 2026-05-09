\# Result Analysis



\## Overview



The simulated buck converter was analyzed under multiple operating conditions to investigate the transition between:

\- continuous conduction mode (CCM),

\- critical conduction mode,

\- and discontinuous conduction mode (DCM).



The analysis demonstrated the influence of:

\- inductance variation,

\- and load resistance variation

on converter operating behavior.



\---



\## CCM Operation Analysis



Under normal design conditions:

\- L = 103.25 µH

\- R = 2.33 Ω



the converter operated in continuous conduction mode.



The obtained waveforms showed:

\- continuous inductor current,

\- stable output voltage,

\- relatively small output ripple,

\- and stable energy transfer.



The output voltage remained close to the required 7 V level with ripple significantly below the assignment limit.



\---



\## Critical Conduction Analysis



Critical conduction operation was achieved using:

\- inductance reduction,

\- and load resistance variation.



As the operating point approached the CCM/DCM boundary:

\- inductor current ripple increased,

\- minimum current approached zero,

\- and converter operation became more sensitive to parameter changes.



The critical conduction waveforms demonstrated the transition region between continuous and discontinuous current conduction.



\---



\## DCM Operation Analysis



Discontinuous conduction mode was achieved by:

\- reducing inductance below the critical value,

\- and increasing load resistance.



The resulting waveforms showed:

\- zero-current intervals,

\- larger ripple,

\- higher peak currents,

\- and discontinuous energy transfer behavior.



The obtained DCM waveforms clearly demonstrated the reduction of stored inductor energy during each switching cycle.



\---



\## Effect of Inductance Variation



Reducing inductance caused:

\- increased current ripple,

\- reduced stored magnetic energy,

\- and earlier current decay.



As inductance decreased:

\- converter operation transitioned from CCM toward DCM.



This behavior agrees with theoretical converter analysis.



\---



\## Effect of Load Resistance Variation



Increasing load resistance reduced output current demand.



As load current decreased:

\- the inductor current decayed faster,

\- causing the converter to approach critical conduction and eventually enter DCM operation.



This demonstrates that converter operating mode depends strongly on loading conditions.



\---



\## Waveform Comparison Summary



| Operating Mode | Current Behavior | Ripple Level | Zero Current Interval |

|---|---|---|---|

| CCM | Continuous | Small | No |

| Critical Mode | Boundary conduction | Moderate | Nearly zero |

| DCM | Discontinuous | Large | Yes |



\---



\## Overall Converter Performance



The simulated buck converter successfully achieved:

\- stable voltage step-down operation,

\- controlled PWM switching,

\- continuous conduction operation,

\- critical conduction transition,

\- and discontinuous conduction behavior.



The obtained results were consistent with theoretical buck converter operation and verified the expected effects of inductance and load variation.

