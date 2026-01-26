
ULTRA SPR — MV Distribution / “High-Voltage Distribution” (Training Primer)

1) MV distribution = 1 kV < U ≤ 52 kV engineering for safety + continuity + selectivity + cost.
2) Design axes: dielectric withstand (Ud/Up) + thermal/electrodynamic withstand (Ir/Ik/Ip).
3) Standards are constraint grammar: they convert hazards into measurable acceptance criteria.
4) Rated voltage Ur > operating voltage; rating ties directly to insulation coordination.
5) Insulation level = power-frequency withstand (50 Hz, 1 min) + lightning impulse withstand (1.2/50 µs).
6) Voltage classes: LV ≤ 1 kV; MV 1–52 kV; HV > 52 kV; use preferred IEC voltage steps.
7) Current classes: Ir (continuous); Isc (fault); Ik/Ith (short-time thermal); Ip/Idyn (peak mechanical).
8) Asymmetrical fault peaks depend on X/R; DC offset drives first-half-cycle stress.
9) Switchgear is role separation: isolate vs switch load vs interrupt fault vs limit energy.
10) Disconnector: isolation only; no fault breaking; interlocks/lockout/padlock embody safety.
11) Switch: breaks load current with defined endurance; limited fault duty.
12) Circuit breaker: interrupts fault current; defined operating sequences; stored-energy mechanism common.
13) Contactor: frequent operations (motors); must be paired with isolation function.
14) Fuse: non-linear I–t energy limiter; limitation curve shapes peak and I²t let-through.
15) Breaking media trade-space: maintenance + footprint + switching overvoltage + environment.
16) Oil: maintenance/pollution legacy burden; space/handling constraints.
17) SF6: strong dielectric/arc behavior; lifecycle now constrained by greenhouse impact.
18) Vacuum: compact, durable; watch switching transient behavior on certain loads.
19) Metal-enclosed MV switchgear = compartmentalized safety architecture (cells within an enclosure).
20) Partition class (PM/PI) defines barrier philosophy between live parts and accessible compartments.
21) Service continuity is formalized by LSC classes: what stays energized during compartment access.
22) Internal arc withstand is a survival spec, not a marketing claim; acceptance is rule-based.
23) Internal arc acceptance: doors stay closed; no fragmentation; no accessible-side holes (≤2 m); no indicator ignition; earthing continuity maintained.
24) Accessibility coding (A/B/C) models human proximity; direction (F/L/R) models exposure geometry.
25) MV network topology is reliability economics encoded in single-line diagrams.
26) Radial feeder: simplest/cheapest; low continuity; fault restoration slower.
27) Open-loop ring: one normally open point; faults isolated then supply restored by switching; automation increases value.
28) Closed-loop ring: bidirectional supply; requires breakers + directional/differential logic for fast isolation.
29) Normal-standby architecture formalizes redundancy; transfer strategy defines interruption behavior.
30) Closed-transition transfer (CTTS): brief overlap to reduce interruption; control-power and CB dynamics matter.
31) Double busbar: segmentation and fault containment; complexity trades for availability.
32) Substation type selection changes responsibility boundaries and metering location (LV vs MV metering).
33) “Inspection / verification / operating rights” can dominate architecture as much as physics.
34) Load survey is the upstream truth: it drives subscription, voltage choice, ratings, cable sizes, fault levels, PF correction.
35) Diversity/utilization factors compress real load behavior into design current assumptions.
36) PF correction uses Qc = P·(tanφ − tanφ′); large kvar often favors MV capacitor placement.
37) Cable sizing is multi-factor: design current Ib + installation/ambient/soil/grouping correction factors.
38) Ampacity is derated by method + temperature + soil conductivity + proximity; parallel runs count as multiple circuits.
39) Cable short-circuit thermal limit follows S = k·Isc·√t; k depends on conductor/insulation assumptions.
40) Conductor–protection coordination invariants: IB ≤ In ≤ Iz and I2 ≤ 1.45·Iz.
41) MV earthing is a triangle: fault-current magnitude vs overvoltage limitation vs first-fault continuity.
42) Unearthed neutral: earth-fault current mainly capacitive (≈3·ω·C·V); first fault may not trip → continuity.
43) Unearthed neutral risk: healthy phases rise toward line-to-line voltage to earth (≈√3) → insulation stress/overvoltage.
44) Solidly earthed: very high earth-fault current; overvoltage controlled; damage energy high; continuity lost; protection simpler.
45) Resistance earthed: compromise; limits current while absorbing overvoltage; earth-fault selectivity often time-graded.
46) Reactance earthed: current limiting with different loss/thermal behavior; common in some public networks; industry risk noted.
47) Resonant earthed (Petersen coil): tune reactor to cancel capacitive earth-fault current; fault current nearly nulled.
48) Earthing choice correlates with network length: long public networks favor current control; shorter industrial networks may favor continuity logic.
49) Overvoltage taxonomy: internal (switching, load variation, ferroresonance, earth faults) vs external (higher-voltage contact, static, lightning).
50) Switching surges originate from arc physics: chopping + restriking + prebreakdown → high dU/dt, HF content.
51) Load disconnection causes regulator-induced voltage excursions; dynamic behavior matters.
52) Ferroresonance: saturated VT reactors + network capacitance → multiple stable high-voltage states; occurs in insulated/high-impedance neutrals.
53) Lightning modeled by standardized impulse wave (1.2/50 µs); protection is surge arrester + coordination.
54) Insulation coordination aligns Ur–Ud–Up so protective devices clamp before equipment dielectrics fail.
55) Overcurrent taxonomy: overload (time-long thermal) vs short-circuit (instant thermal + mechanical).
56) Short-circuit current is symmetric + DC offset; X/R sets asymmetry and peak forces.
57) Equipment selection from Isc: breaking capacity + making capacity + thermal withstand + dynamic withstand for CB/sensors/busbars/cables.
58) Protection relays are cyber-physical controllers: measure + decide + trip + log + communicate.
59) Time-overcurrent: definite-time vs IDMT; grading margins and pickup ratios enforce coordination feasibility.
60) Selectivity toolbox: current grading, time grading, logical blocking/pilot, directional, differential, residual-current schemes.
61) Directional protection uses V–I phase angle to separate fault direction in rings/parallel feeders.
62) Differential protection compares boundary currents; isolates internal faults in loops, transformers, machines, busbars.
63) Arc fault = plasma path + extreme heat + pressure + radiation + molten metal; human + asset fatality mechanism.
64) Damage scales with arcing time; incident energy behaves like I²t; faster clearing collapses damage area.
65) Arc protection = fast light sensing + current validation + immediate trip path; targets sub-60 ms clearing.
66) Arc-flash safety framework defines approach boundaries and PPE categories; procedure is part of protection.
67) Transformer technology split: oil-immersed (breathing vs sealed) vs dry-type (cast resin); driven by cooling + environment + installation.
68) Oil-immersed internal fault sensing: gas/pressure/temperature logic (e.g., Buchholz/DGPT family) + thermal sensors.
69) Dry-type relies on embedded thermal protection; insulation system and encapsulation define behavior.
70) Transformer primary protection layers: short-circuit, overload, earth fault/tank leakage, internal fault (incl. differential at higher power).
71) Paralleling constraints: compatible ratings, same source, similar cable impedance, matching vector group, close %Z.
72) Tap changing: NLTC (off-circuit) for stable systems; OLTC (on-load) is the actuator for regulated voltage under fluctuating load.
73) Core mental model: MV systems are designed by controlling where energy flows during abnormal events.
74) Design success metric: keep fault energy local, keep healthy parts energized, keep humans outside the hazard envelope.
