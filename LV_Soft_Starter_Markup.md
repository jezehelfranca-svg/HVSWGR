# LV Soft Starter Specification – Markup from GS EP ELE 123 (VSD)

**Source Document:** GS EP ELE 123 – Low Voltage Variable Speed Drive, Rev. 02 (11/2020)
**Target Document:** GS EP ELE 124 – Low Voltage Soft Starter, Rev. 00 (02/2026)
**Markup Reference:** `Low%20Voltage%20Soft%20Starter_marked_for_soft_starter.pdf`

---

## Summary of Changes

This markup document records all modifications made when adapting the VSD specification (GS EP ELE 123) into the LV Soft Starter specification (GS EP ELE 124). Sections marked as "struck through" in the original marked PDF are identified as NOT APPLICABLE for soft starters and have been removed or replaced.

---

## Global Changes (Throughout Document)

| Change Type | From (VSD) | To (Soft Starter) |
|-------------|-----------|-------------------|
| Document Number | GS EP ELE 123 | GS EP ELE 124 |
| Title | Low Voltage Variable Speed Drive | Low Voltage Soft Starter |
| Abbreviation | VSD | SS (Soft Starter) |
| Data Sheet ref | DS EP ELE 123 | DS EP ELE 124 |
| Primary IEC standard | IEC 61800 (Parts 2; 3; 5-1) | IEC 60947-4-2 |
| All terminology | "Variable Speed Drive" / "VSD" | "Soft Starter" |

---

## Section-by-Section Markup

### Section 1: Scope
- **MODIFIED:** Changed "variable speed drives (VSD)" → "soft starters"
- **MODIFIED:** Changed "DC variable speed drives" → "DC motor starters"

### Section 2: Reference Documents
- **REMOVED:** IEC 60146 (Semiconductor converters) – *Not applicable, VSD-specific*
- **REMOVED:** IEC 61800 (Parts 2; 3; 5-1) – *Replaced with IEC 60947-4-2*
- **REMOVED:** EN 50598-2 – *Energy efficiency for power drive systems, VSD-specific*
- **ADDED:** IEC 60947-4-2 – *Specific standard for AC semiconductor motor controllers and starters*

### Section 3: Applicability
- **MODIFIED:** Removed "wall mounted" installation option – *Soft starters are typically cabinet-mounted*

### Section 4: Definitions of Terms
- **REMOVED:** dV/dt (Voltage instantaneous rate of change) – *VSD-specific PWM concern*
- **ADDED:** SS (Soft Starter)

### Section 5: Scope of Supply
- **MODIFIED:** Updated data sheet reference from DS EP ELE 123 to DS EP ELE 124

### Section 6.2: Definition of Equipment
- **REMOVED:** "wall mounted VSD unit" option – *Not typical for soft starters*
- **MODIFIED:** By-pass description changed from "allows VSD troubleshooting without affecting operation" → by-pass contactor for continuous running at full speed after start, rated for continuous duty

### Section 6.3.1: Voltages and Neutral Earthing
- **MODIFIED:** "power a low voltage asynchronous motor" → "start and control a low voltage asynchronous motor"

### Section 6.3.3: Output Voltage of the VSD
- **REMOVED ENTIRELY** – *Soft starters do not have a variable output voltage specification in the same sense*

### Section 6.4: Technical Requirements
- **REMOVED:** Speed variation range, minimum speed, forced ventilation for slow speeds – *VSD-specific continuous speed control concerns*
- **REMOVED:** THDi harmonic current distortion requirements – *Soft starters do not generate significant harmonics during running (thyristors fully conducting)*
- **REMOVED:** dV/dt filters, sine filters, motor insulation voltage protection – *VSD-specific PWM waveform concerns*
- **REMOVED:** Motor reinforced insulation as alternative to filters – *VSD-specific*
- **REMOVED:** Semiconductor converter requirements per IEC 60146 – *VSD-specific*
- **REMOVED:** IE2 efficiency class per EN 50598-2 – *VSD-specific*
- **REMOVED:** Overvoltage category III per IEC 61800-5-1 – *Replaced with IEC 60947-4-2*
- **REMOVED:** Climatic condition class 3K3 per IEC 61800-2 – *Covered by IEC 60947-4-2*
- **REMOVED:** Wall-mounted VSD fuse provisions (Appendix 3 reference) – *Removed wall mount option*
- **ADDED:** IEC 60947-4-2 compliance requirement

### Section 6.5: Performance Requirements
- **REMOVED:** "Only one operating quadrant" – *VSD-specific*
- **REMOVED:** Speed/torque curve and starting time overload (150% or 110% for 60s) – *VSD-specific continuous operation*
- **REMOVED:** ±1% speed variation at rated operating point – *No speed regulation in soft starter*
- **REMOVED:** Frequency variation range at output – *No frequency output in soft starter*
- **REMOVED:** Voltage/frequency ratio adjustment – *VSD-specific V/f control*
- **REMOVED:** Remote speed adjustment by 4-20 mA signal – *No continuous speed control*
- **REMOVED:** Voltage dip operation (70% for 250 msec) – *VSD-specific ride-through*
- **REMOVED:** Restart after momentary power loss – *VSD-specific*
- **ADDED:** Voltage ramp soft starting with adjustable starting voltage and ramp time
- **ADDED:** Current limiting soft starting capability
- **ADDED:** Adjustable deceleration (soft stop) ramp time
- **ADDED:** Starting current limitation (adjustable, typically 2 to 4 × FLA)
- **ADDED:** Specified number of starts per hour capability
- **ADDED:** Motor starting torque suited to driven machine requirements

### Section 6.6: Power Cables
- **REMOVED:** Shielded cable requirement for EMC – *VSD-specific EMI from PWM switching*
- **REMOVED:** Waveform reflection and voltage signal distortion concerns – *VSD/PWM-specific*
- **REMOVED:** dV/dt filter requirement – *VSD-specific*

### Section 6.8: Protection Devices and Information
- **REMOVED (VSD-specific protections):**
  - DC Bus over voltage
  - Rectifier over current
  - Inverter over current
  - Inverter overvoltage
  - Inverter overload
  - Converter ground fault
- **ADDED (Soft Starter-specific protections):**
  - Thyristor (SCR) over temperature
  - Thyristor (SCR) short circuit
  - Thyristor (SCR) open circuit
  - Heatsink over temperature
  - Phase loss / phase reversal
  - Locked rotor
  - Excessive number of starts
- **MODIFIED (Front panel information):**
  - Removed: Output frequency, Speed reference, Output speed, Output active power, Output voltage
  - Changed: "Output current" → "Motor current"
  - Changed LED indicators from "running" → "Starting (ramping)" and "Running (at full speed / bypassed)"
  - Changed 4-20 mA signal from "motor speed" → "motor current"

### Section 6.10: Electromagnetic Compatibility
- **MODIFIED:** Changed IEC 61800-3 criterion A → IEC 60947-4-2

### Section 7.1: Metal-enclosed Cabinet
- **NO CHANGE** – Applicable as-is

### Section 7.9: HMI
- **NO CHANGE** – Applicable as-is

### Section 7.11: Manufacturer's Nameplate
- **REMOVED:** "Rated input and output voltages" → "Rated input voltage"
- **REMOVED:** "Rated output power (kW)" → "Rated motor power (kW)"
- **ADDED:** Rated current (A)
- **ADDED:** Utilisation category (AC-53)

### Section 8.1: Factory Acceptance Tests
- **MODIFIED:** Changed IEC 61800-2 and IEC 61800-5-1 → IEC 60947-4-2

### Section 8.4: List of Tests
- **MODIFIED:** Changed "Routine tests as per IEC 61800-2 or IEC 61800-5-1" → "IEC 60947-4-2"
- **MODIFIED:** Changed "Adjustment and functional tests of the VSD coupled with the motor" → "Functional tests of the soft starter coupled with the motor"

### Section 10: Installation
- **REMOVED:** Wall-mounted VSD frame requirement – *Wall mount option removed*

### Section 13: Documentation List (Appendix 1)
- **REMOVED:** "Preliminary harmonic study at line side" – *VSD-specific*
- **REMOVED:** "VSD torque-speed curve in all speed range superimposed to load curve" 
- **ADDED:** "Soft starter starting current-time curve superimposed to motor thermal limit curve"

### Appendices
- **REMOVED:** Appendix 3 (Schematic – VSD wall mounted) – *Wall mount not applicable*
- **REMOVED:** Appendix 5 (Data Sheets DS EP ELE 123) → Replaced with Appendix 4 (DS EP ELE 124)
- **RENUMBERED:** Appendices reduced from 5 to 4

---

## Sections Retained Without Modification

The following sections were carried over from GS EP ELE 123 with only terminology changes (VSD → Soft Starter):

- Section 6.1 – Service conditions (all sub-sections)
- Section 6.3.2 – Electrical system variations
- Section 6.7 – Temperature sensors
- Section 6.9 – Noise levels  
- Section 6.11 – Regulatory requirements
- Section 7.1 through 7.8 – All construction requirements
- Section 7.10 – Anti-condensation heating
- Section 8.2, 8.3 – On-site tests and reports
- Section 9 – Packaging and shipment
- Section 11 – Spare parts (all sub-sections)
- Section 12 – Documentation
