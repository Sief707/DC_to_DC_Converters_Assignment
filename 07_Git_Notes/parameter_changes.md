# Parameter Change Tracking

## Updated Stable CCM Design

| Parameter | Value |
|---|---|
| Vin | 24 V |
| Vo | 7 V |
| Io | 3 A |
| fs | 10 kHz |
| Duty Cycle | 0.292 |
| Rload | 2.33 Ω |
| L | 103.25 µH |
| C | 857.14 µF |

## PWM Settings

| Parameter | Value |
|---|---|
| Switching Frequency | 10 kHz |
| Period | 100 µs |
| Duty Cycle | 29.2% |
| Stop Time | 1 s |

## Device Modeling

| Device | Parameter | Value |
|---|---|---|
| Diode | Forward Voltage Vf | 0 V |
| Diode | Ron | 0.001 Ω |
| MOSFET | Ron | 0.1 Ω |

## Planned Future Variations

### Critical Conduction
- Reduce inductance toward critical inductance value

### DCM by Inductor Reduction
- Reduce inductance below critical value

### DCM by Load Variation
- Increase load resistance