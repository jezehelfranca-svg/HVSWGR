
# ⚡ SPR Engineering Brief — Relay Protection Coordination (Rev. 4A)

**Document purpose.** This brief expands the previously issued SPR Compression into a field‑ready, engineering‑actionable package covering objectives, assumptions, setting methodology, coordination checks, arc‑flash scheme, FAT/SAT verification, and acceptance criteria for the AMIRAL (PKG‑1) MFC electrical distribution (13.8 kV / 4.16 kV / 0.48 kV). citeturn1search2

---

## 0) Executive Summary
- **Goal**: Deliver selective, sensitive, and fast protection across 13.8 kV, 4.16 kV, and 0.48 kV systems, while maintaining upstream/downstream discrimination and enabling safe ATS/synchronism operations. citeturn1search2
- **Standards & Tools**: ETAP v22.0.2 study basis; IEC/ANSI protection practice per AMIES‑P‑100/114, IEEE 242/399/141, IEC 60909. Relays: **SEL‑451, SEL‑751, SEL‑710, SEL‑849, ELR‑3C**. citeturn1search2
- **Coordination margins**: **0.35–0.50 s** in normal topology; **0.25 s** single‑ended. No instantaneous phase (50P) on incomers. Ground protection layered (tank/neutral/residual). citeturn1search2
- **System fault references** (drive settings): **13.8 kV ~24 kA (max) / ~11.7 kA (min); 1φ‑G 400 A. 0.48 kV ~70.9 kA (max).** citeturn1search2

---

## 1) System Context & Assumptions
1. **Network**: Secondary‑selective architecture with redundant incomers and normally‑open bus ties on MV/LV switchgears; ATS and synch‑check interlocks enabled. citeturn1search2
2. **Sources/Transformers**: 34.5/14.5 kV 50/63 MVA feeding 13.8 kV; step‑downs 13.8/4.4 kV (16/20 MVA) and 13.8/0.5 kV (3.15 MVA); generator incomers at 4.16 kV where applicable. citeturn1search2
3. **Grounding**: MV neutral via **low‑resistance** grounding (Ig ≈ **400 A** reference). LV earth‑leakage via ELR/SEL‑849. citeturn1search2
4. **CT/PT Infrastructure**: Typical CTs 4000/5 (MV incomer), 1250/5 (MV feeder), 600/5 or 200/5 (motors), ZCT 50/5; PTs 13.8/√3→110/√3. citeturn1search2

---

## 2) Protection Philosophy (Top‑down)
**2.1 Selectivity & Speed**  
- Upstream devices intentionally slower on inverse time; no 50P on incomers to preserve coordination and avoid false trips during motor starts or downstream faults. citeturn1search2

**2.2 Sensitivity (Ground Faulting)**  
- Dual ground sensing for transformers (tank 50G and neutral 51NT), feeders (51N/51G), and LV ELR—ensures detection of high‑impedance faults and transformer tank faults. citeturn1search2

**2.3 Stability**  
- Motor protective elements (49, 46, 51LR, 27D, 66) set to avoid nuisance during start/jog, respecting vendor LRC and thermal withstand. citeturn1search2

**2.4 Operational Continuity**  
- ATS logic gated by undervoltage (27‑2A @ 90% V, 0.5 s) and bus residual undervoltage monitors on ties (27‑R1/R2 @ 20% V). Synch‑check (25) enforces ΔV 10%, Δφ 10°, slip 0.05 Hz, breaker close ~8 cycles. citeturn1search2

---

## 3) Settings Methodology (Abstract → Concrete)
**3.1 Phase Overcurrent (51)**  
- **Pickup**: \(I_{p} = K \cdot (I_{FLA} \cdot 5/CT)\) with **K = 1.25–1.5** (feeders/transformers) and **≥1.05** for motors. Curve: **IEC Very Inverse (C2)**. Time dial selected so **t(M_{max})** achieves the specified coordination margin at **M = I_{fault}/I_p** using \( t = 13.5\,TD/(M-1) \). citeturn1search2

**3.2 Instantaneous (50)**  
- **Incomers**: not used. **Feeders/Transformers**: set ≈ **1.75 × through‑fault** on CT‑secondary; delay 0–0.05 s as specified. **Motors**: set above first inrush and above motor contribution to remote faults. citeturn1search2

**3.3 Ground (50N/51N/50G/51G)**  
- Reference Ig = **400 A** at MV. Typical picks: **50G ≈ 0.7·Ig**, **51G ≈ 0.3·Ig** (residual), **51N ≈ 0.2·Ig** (core‑balance where applied), with delays 0.4–0.75 s coordinated upstream/downstream. Transformer **tank 50G = 0.3·Ig; 51NT = 0.6·Ig** fast IDMT. citeturn1search2

**3.4 Voltage & Synch**  
- **27‑1A Trip** 80% V (1–3 s), **27‑2A ATS block** 90% V (0.5 s), **59** 120% V (2 s), **25** ΔV 10% / Δφ 10° / slip 0.05 Hz / 8 cycles close. citeturn1search2

**3.5 Arc‑Flash (50AF)**  
- **Pickup 3–9 A** (sec) with optical **POINT/FIBER** sensors; **TOL1P = 3%**. Trips via high‑speed scheme to minimize incident energy while preserving selectivity with upstream inverse curves. citeturn1search2

---

## 4) Critical Settings (Concrete Values)
> Representative values below; full tables are in the Rev. 4A study.

### 4.1 13.8 kV Incomers — SEL‑451
- **51P**: pickup **≈3.27 A**, **C2**, **TD ≈ 0.55** (A/B).  
- **50G**: **0.35 A @ 45 cycles**; **51G**: **0.25 A, TD 0.06**.  
- **27‑1A**: **50.4 V** (trip); **27‑2A**: **56.9 V** (ATS block); **59**: **57.6 V**. citeturn1search2

### 4.2 13.8 → 4.4 kV Transformers — SEL‑751 (Feeder) + SEL‑751 (Neutral)
- **50P**: **43.72 A** (inst); **51P**: **4.02 A**, **C2**, **TD 0.50**.  
- **50N** (primary): **4 A / 0.05 s**.  
- **51NT** (secondary): **6 A**, **C2**, **TD 0.05–0.16** depending on bank.  
- **Tank 50G**: **3.0 A / 0.2 s**. citeturn1search2

### 4.3 13.8 → 0.5 kV Transformers — SEL‑751
- **50P**: **37.19 A**; **51P**: **2.47 A**, **TD 0.73**.  
- **50N**: **4 A / 0.05 s**. citeturn1search2

### 4.4 MV Motors — SEL‑710 (e.g., 1750 kW)
- **51**: **1.05 × FLA**; **51LR**: **3× FLA / 2 s**; **46**: **20% / 3–5 s**; **49**: **1.05× FLA** tuned above start curve; **27D**: **76% V / 3 s**. citeturn1search2

### 4.5 Outgoing MV Feeders to SS220101 — SEL‑751
- **50P**: **100 A** (definite, 0 s).  
- **51P**: **3.43 A**, **C2**, **TD 0.98**.  
- **50N**: **20 A / 0.4 s**; **51N**: **8 A / TD 0.12**. citeturn1search2

### 4.6 LV (480 V) SSG/MCC Feeders — SEL‑751/SEL‑849/ELR‑3C
- **51**: **150% × transformer site rating**; **50**: **20–40% × I3φ,max** depending on panel topology.  
- **64 (ELR)**: **1–3 A**, **0.05–0.2 s** (panel ≤1 A for loads, 3 A for power panels). citeturn1search2

---

## 5) Coordination Checks (What to verify)
**5.1 Time‑Current Curves**  
- Confirm **Δt ≥ 0.35–0.50 s** at **normal maximum transient** between each device pair (feeder ↔ incomer; motor ↔ feeder; LV branch ↔ MCC; etc.). For single‑ended operation, **Δt ≥ 0.25 s**. citeturn1search2

**5.2 Motor Starts**  
- Ensure **51** clearing time sits **above start curve** and **below stall withstand**; **50** not asserted during inrush; **51LR** not asserted during normal acceleration (per vendor start time). citeturn1search2

**5.3 Ground Selectivity**  
- **51N/51G** of feeders must clear before incomer **51G/51N** for faults downstream; transformer **51NT** must coordinate with feeder **51N**. citeturn1search2

**5.4 Arc‑Flash Scheme**  
- Verify optical sensors coverage; **50AF** supervised by current (pickup 3–9 A) to avoid spurious trips; ensure upstream inverse curves don’t under‑reach AF trip times at minimum fault levels. citeturn1search2

**5.5 ATS & Synchro‑Check**  
- **27‑2A** blocks ATS until bus residual falls below **20% V** (27‑R1/R2) and **25** criteria satisfied: ΔV 10%, Δφ 10°, slip ≤0.05 Hz, breaker close time configured (≈8 cycles). citeturn1search2

---

## 6) Field Acceptance Criteria (Measurable)
1. **Relay burdening & polarity**: CT/VT ratios and polarity match settings (samples: 4000/5, 1250/5, 600/5, 50/5). **Acceptance**: nameplate ↔ settings一致; secondary injection scaling correct within **±1%**. citeturn1search2
2. **Pickup accuracy**: Secondary injection verifies 51P/51N/51G pickups within **±5%** of set value; **50** definite within **±1 step**. citeturn1search2
3. **Time dial**: IDMT timing at **M‑point** (study point) within **±7%** vs. calculated \( t=13.5·TD/(M−1) \). citeturn1search2
4. **Coordination margin**: Demonstrated by overlaying downstream vs upstream TCC in relay or ETAP; **Δt ≥ specified**. citeturn1search2
5. **Voltage elements**: 27/59 pick‑ups at **80/90/120%** thresholds, time delays within **±0.1 s**. 25 close permissive validated using simulated sources. citeturn1search2
6. **Arc‑flash**: Optical + amp supervision functional; trip within **≤40 ms** from detection path; zone coverage drawings markup signed. citeturn1search2
7. **Interlocks**: ATS inhibit and bus‑tie logic observed per sequence test; no parallel close unless **25** satisfied. citeturn1search2

---

## 7) FAT / SAT Verification Plan (Actionable)
**FAT (Panel/Vendor works)**  
- Review wiring vs. **CT/PT ratio tables**; simulate secondary faults for 51/51N/51G; verify **27/59/25** logic; arc‑flash sensor loop tests. Outputs: signed FAT sheets and exported **.set** files from SEL‑451/751/710/849. citeturn1search2

**SAT (Site)**  
- Primary injection at selected feeders to validate CT circuits; system‑level ATS sequence (loss of source, residual check, tie close under **25**); motor cold/hot start permissives (66), and thermal reset behavior (49). Archive: **as‑left settings**, **event reports**, and **oscillography** of staged trips. citeturn1search2

---

## 8) Risk Register (Compressed)
| Risk | Cause | Impact | Mitigation / Test |
|---|---|---|---|
| Loss of selectivity on MV ground faults | 51N/51G mis‑graded vs 51NT | Unnecessary upstream trip | Re‑time TD per C2; verify M‑point (Ig/Ip); injection tests. citeturn1search2 |
| Incomer nuisance trip | 50P applied or 51 too low | Plant blackout | Keep 50P **OFF**; 51 at ≥1.25× transformer FLA; verify with through‑fault. citeturn1search2 |
| Motor start trip | 50P/51LR too low | Process upset | Elevate 50 above inrush; 51LR = 3×FLA/2 s; validate vs vendor LRC/time. citeturn1search2 |
| AF false trip | Optical noise or sunlight | Unwanted outage | Use current supervision (3–9 A) + TOL = 3%; zone walkdown. citeturn1search2 |
| ATS mis‑operation | UV/synch set wrong | Bus tie close out‑of‑sync | Enforce 27‑2A = 90% V, 25 = ΔV/Δφ/slip per spec; perform black start test. citeturn1search2 |

---

## 9) Deliverables & Handover
- **SPR Settings Book** (per relay) — one‑pager extracts from Rev.4A settings. citeturn1search2
- **Coordination Plots** (ETAP TCC PDFs) — upstream/downstream overlays at normal & single‑ended. citeturn1search2
- **FAT/SAT Check Sheets** (this brief, §6–7). citeturn1search2
- **As‑Left SEL files (.set)** and **ser event captures**. citeturn1search2

---

## 10) Appendix — Quick Reference Tables

### A. Typical Pickups & Time Dials (MV)
| Function | Typical Value | Notes |
|---|---|---|
| 13.8 kV Incomer 51P | **3.27 A**, C2, TD **0.55** | Based on 1.25× transformer FLA. citeturn1search2 |
| 13.8→4.4 kV Feeder 51P | **4.02 A**, C2, TD **0.50** | Through‑fault M≈6.2 → ~1.3 s. citeturn1search2 |
| 13.8→0.5 kV Feeder 51P | **2.47 A**, C2, TD **0.73** | Through‑fault M≈8.6 → ~1.3 s. citeturn1search2 |
| MV Feeder to SS220101 51P | **3.43 A**, C2, TD **0.98** | Target 0.5 s at M≈27.4. citeturn1search2 |

### B. Ground Protection Anchors
| Function | Value | Coordination Target |
|---|---|---|
| Transformer Tank 50G | **3.0 A / 0.2 s** | Fast tank fault clearing. citeturn1search2 |
| Transformer 51NT | **6–7 A / C2 / TD 0.05–0.16** | ≤1.1 s at Ig (coord. to feeders). citeturn1search2 |
| Incomer 50G/51G | **0.35 A / 0.25 A (TD 0.06)** | Grade to feeders’ 51N/51G. citeturn1search2 |

### C. Voltage & Synchro
| Function | Setpoint |
|---|---|
| 27‑1A (Trip) | **80% V (e.g., 50.4 V sec)** citeturn1search2 |
| 27‑2A (ATS block) | **90% V (e.g., 56.9 V sec)** citeturn1search2 |
| 59 (Trip) | **120% V (e.g., 57.6 V sec)** citeturn1search2 |
| 25 (Synch) | **ΔV 10%, Δφ 10°, slip 0.05 Hz, close 8 cycles** citeturn1search2 |

---

### Notes
- All figures/values are **extracted from** and **traceable to** the Rev. 4A “Relay Protection Coordination” document dated **25‑Feb‑2026**. Use this brief as an operational aid; **the Rev. 4A study remains the controlling document**. citeturn1search2

