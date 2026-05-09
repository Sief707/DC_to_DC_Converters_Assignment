\# Simulink Implementation Notes



\## Baseline CCM Parameters



| Parameter | Value |

|---|---|

| Vin | 24 V |

| Vo | 7 V |

| fs | 20 kHz |

| Duty Cycle | 0.292 |

| Rload | 2.33 Ω |

| L | 300 µH |

| C | 100 µF |



\## Simulation Configuration



\- Open-loop operation

\- PWM pulse control

\- Discrete solver

\- Sampling time = 10e-6 sec

\- Maximum simulation duration = 10 switching cycles



\## Initial Power Stage Construction



The open-loop buck converter topology was implemented using Simscape Electrical Specialized Power Systems.



Implemented components:

\- DC voltage source

\- MOSFET switch

\- Freewheeling diode

\- Inductor

\- Capacitor

\- Resistive load

\- Current measurement blocks

\- Voltage measurement blocks

\- PWM pulse generator

\- powergui block



The simulation environment was configured using discrete mode with sampling time of 10e-6 sec according to assignment instructions.



\## PWM Configuration



The MOSFET switching signal was generated using a pulse generator block.



PWM parameters:



\- Amplitude = 1

\- Switching frequency = 20 kHz

\- Period = 50 µs

\- Duty cycle = 29.2%



The duty cycle was selected according to the theoretical buck converter relationship:



D = Vo / Vin



\## Measurement Architecture



Measurement blocks were added to monitor converter operation during simulation.



\### Voltage Measurements

\- Input voltage Vin

\- Output voltage Vo

\- MOSFET switching voltage VSW



\### Current Measurements

\- MOSFET current ISW

\- Inductor current IL

\- Diode current ID



Scopes were organized into:

\- Current waveforms

\- Voltage waveforms

\- PWM control signal

