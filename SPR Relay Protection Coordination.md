# ⚡ SPR Compression — Relay Protection Coordination (Rev.4A)

## 1. Scope (Compressed)
Complete relay protection coordination for **13.8 kV / 4.16 kV / 0.48 kV** distribution, covering:
- Transformers
- Bus-tie & incomers
- Outgoing feeders
- MV motors
- LV MCC & SSG feeders

(Extracted from document) citeturn1search2

## 2. System Fault Levels
- 13.8 kV: Max ~24 kA, Min ~11.7 kA, Ground 400 A citeturn1search2
- 480 V: Max ~70.9 kA, Min ~34.2 kA, Ground 3–5 A citeturn1search2

## 3. Protection Core Logic
### Overcurrent
- 50 instantaneous: Not used on incomers.
- 51 pickup: 1.25–1.5× FLA; IEC C2 curve. citeturn1search2

### Ground Fault
- 50G/50N: 0.1–0.7 × Ig.
- 51N/51G: 20–30% Ig; time dial 0.06–0.75 s. citeturn1search2

### Voltage Functions
- 27-1A: 80% V, 1–3 s.
- 27-2A: 90% V, 0.5 s.
- 59: 120% V, 2 s. citeturn1search2

### Synchronism Check
- ΔV 10%, ΔΦ 10°, slip 0.05 Hz, 8 cycles. citeturn1search2

## 4. Arc Flash (50AF)
- Trip 3–9 A, POINT/FIBER sensor, TOL1P = 3%. citeturn1search2

## 5. CT/PT Ratios
- Incoming: 4000/5A
- Feeder: 1250/5A
- Motors: 600/5A, etc.
- PT: 13.8/√3 → 110/√3. citeturn1search2

## 6. Formulas
### Phase OC Pickup
I = K × (Ibase × 5 / CT) with K=1.25–1.75. citeturn1search2

### IEC Time Dial
 t = (13.5 × TD) / (M−1). citeturn1search2

## 7. Key Settings Summary
### 13.8 kV Incomers (SEL-451)
- 51P1P ≈ 3.2 A, TD ≈ 0.55.
- 50G = 0.35 A, 51G = 0.25 A TD 0.06.
- UV 50.4 V, OV 57.6 V. citeturn1search2

### Transformer 16/20 MVA
- 50P1P = 43.7 A
- 51P1P = 4.0 A, TD 0.50
- 50N = 4 A, delay 0.05
- 51NT = 6 A, TD 0.05 citeturn1search2

### MV Motors
- LRC ≈ 5–6×FLA, 51LR 3×FLA @ 2 s
- 46 = 20% imbalance
- 49 = 105% thermal
- 27D = 76% V @ 3 s citeturn1search2

## 8. Coordination Philosophy
- Selectivity margin 0.35–0.5 s MV.
- No 50 on incomers.
- Arc‑flash bypass via optical + current.
- Motor thermal > start curve, < stall curve. citeturn1search2

