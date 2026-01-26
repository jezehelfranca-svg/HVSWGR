
ULTRA SPR — LV & MV Drive (Inverter / VFD) Solutions (NO LINKS)

1) A drive system is a controlled energy conversion chain: grid → transformer → rectifier (AC–DC) → DC bus → inverter (DC–AC) → cable → motor → gearbox/load → feedback/control.
2) A VFD (VSD / AC drive / inverter) controls motor speed by varying output frequency and voltage; frequency is directly tied to RPM.
3) Three‑phase motors use three windings phase‑shifted by 120° to create a rotating magnetic field; rotor follows the resultant rotating field.
4) Motor plate data (V, A, kW, cosφ, frequency, poles) is the baseline for drive sizing, protection, and control tuning.

5) Star/Delta wiring trades voltage and starting current: star reduces starting current; delta supports higher starting torque at lower voltage.
6) Synchronous speed depends on frequency and number of poles; induction motors run below synchronous speed due to slip.
7) Slip quantifies the speed difference between rotating field and rotor; slip can’t be zero in a working induction motor.
8) Torque is the mechanical driving force; motor power relates to torque and speed (P ∝ T × ω).

9) Electrical power in three‑phase loads uses the √3·U·I·cosφ form; efficiency is mechanical output divided by electrical input.
10) Motor losses split across stator, rotor, core, friction/windage, and stray load losses; larger motors typically show smaller relative efficiency spread.

11) Starting methods exist because DOL inrush and torque shock can be excessive; VFD is the preferred solution when speed control or reduced stress is required.
12) Wye‑Delta starting reduces voltage to ~57.7% during start, reducing starting torque roughly with V²; transfer to delta occurs around ~80% speed.

13) VFD internal structure is functionally three blocks: rectifier bridge, DC bus (energy storage), inverter (PWM switching).
14) A six‑pulse rectifier conducts in segments over each cycle, producing DC bus ripple and characteristic input harmonics.
15) VFD output is PWM, not a true sine; a sine waveform is only a conceptual reference.

16) Switching (carrier) frequency is a multi‑objective knob: higher carrier reduces audible noise and can improve motor smoothness but increases inverter losses and heating.
17) Lower carrier reduces inverter heating and can reduce stress on winding insulation, but increases audible noise and can increase current distortion.
18) Higher carrier can increase dv/dt spikes, radiated noise, and motor heating; it can also confuse some instruments (measurement anomalies).
19) Total harmonic current distortion THDi is computed from harmonic RMS components relative to the fundamental; higher measured harmonic order increases accuracy of THD reporting.

20) Motor control with drives has two main speed regions: constant torque region (U/F constant) and constant power region (field weakening above base speed).
21) Different loads require different torque–speed profiles: constant torque (conveyors, hoists, mixers) vs quadratic torque (fans, centrifugal pumps) vs specialized profiles (winders, machine tools).
22) Four‑quadrant operation captures motoring and generating in forward and reverse; deceleration can regenerate energy into the DC bus.

23) When regenerating energy raises DC bus voltage beyond acceptable limits, dynamic braking is used to dissipate energy.
24) Dynamic braking uses a brake chopper (IGBT + control) to switch an external resistor across the DC link when voltage exceeds a threshold.
25) A practical rule-of-thumb: inherent motor+drive losses can absorb a limited braking power; if required braking torque percentage exceeds a threshold, add a resistor + chopper.
