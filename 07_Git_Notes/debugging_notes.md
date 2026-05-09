\# PWM Generator Notes



Attempted sample-based pulse generator configuration.



Issue:

\- Sample-based mode requires integer sample counts rather than time values or percentages.



Decision:

\- Returned to time-based PWM configuration because it is simpler and fully compatible with the assignment requirements and discrete powergui simulation.

# Frequency Redesign Notes

The original converter design used:
- fs = 20 kHz

Issue:
- the assignment constrained the simulation to a discrete step size of 10e-6 sec,
- resulting in insufficient switching resolution at 20 kHz.

Updated design:
- switching frequency reduced to 10 kHz,
- switching period increased to 100 µs,
- providing 10 simulation samples per switching cycle.

Updated component values:
- L = 103.25 µH
- C = 857.14 µF

Additional correction:
- diode forward voltage was reduced to zero to approximate ideal converter behavior and achieve the target output voltage near 7V.



