# Buck Converter Design Calculations

## Given Specifications

- Input Voltage = 24 V
- Output Voltage = 7 V
- Output Current = 3 A

---

## Design Assumptions

- Ideal buck converter operation
- Continuous conduction mode (CCM)
- Discrete simulation with sample time = 10e-6 sec
- Switching frequency selected as 10 kHz
- Output voltage ripple maintained below 0.5 V

---

## Output Power

Po = Vo × Io

Po = 21 W

---

## Load Resistance

R = Vo / Io

R = 7 / 3

R = 2.33 Ω

---

## Duty Cycle

:contentReference[oaicite:1]{index=1}

D = 7 / 24

D = 0.292

Duty cycle is approximately 29.2%.

---

## Switching Frequency Selection

The assignment constrains the simulation to a discrete sample time of:

Ts = 10e-6 sec

For accurate switching simulation:

:contentReference[oaicite:2]{index=2}

Thus:

Tsw ≥ 100 µs

Therefore:

:contentReference[oaicite:3]{index=3}

fs ≤ 10 kHz

A switching frequency of 10 kHz was selected.

---

## Minimum Inductance for CCM

:contentReference[oaicite:4]{index=4}

Substituting:

- D = 0.292
- R = 2.33 Ω
- fs = 10 kHz

Lmin ≈ 82.6 µH

---

## Selected Inductance

To ensure continuous conduction mode:

Ldesign = 1.25 × Lmin

Ldesign ≈ 103.25 µH

---

## Output Voltage Ripple

Target ripple voltage:

ΔVo = 0.07 V

---

## Capacitor Design

:contentReference[oaicite:5]{index=5}

Substituting:

- Io = 3 A
- fs = 10 kHz
- ΔVo = 0.07 V

C ≈ 857.14 µF

---

## Final Selected Parameters

| Parameter | Value |
|---|---|
| Vin | 24 V |
| Vo | 7 V |
| Io | 3 A |
| fs | 10 kHz |
| Duty Cycle | 29.2 % |
| R | 2.33 Ω |
| L | 103.25 µH |
| C | 857.14 µF |

---

## CCM Verification

Since:

Ldesign > Lmin

the converter operates in Continuous Conduction Mode (CCM).