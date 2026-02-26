# General Specification

**GS EP ELE 124**

## Low Voltage Soft Starter

| Rev. | Date | Purpose of the revision |
|------|---------|-------------------------|
| 00 | 02/2026 | First issue – Adapted from GS EP ELE 123 (LV Variable Speed Drive) |

**Owning entity:** DSO/IP/TEC
**Managing entity:** DSO/IP/TEC/EIS

> *This document is the property of TOTAL S.E., it contains confidential information which may not be disclosed to any third party, reproduced, stored or transmitted without the prior written consent of TOTAL S.E.*
> *The information contained in this document does not substitute for applicable laws and regulations.*

---

## Contents

1. [Scope](#1-scope)
2. [Reference documents](#2-reference-documents)
3. [Applicability](#3-applicability)
4. [Definitions of terms](#4-definitions-of-terms)
5. [Scope of supply](#5-scope-of-supply)
6. [Design](#6-design)
   - 6.1 Service conditions
   - 6.2 Definition of the equipment
   - 6.3 System voltage
   - 6.4 Technical requirements
   - 6.5 Performance requirements
   - 6.6 Power cables
   - 6.7 Temperature sensors
   - 6.8 Protection devices and information
   - 6.9 Noise levels
   - 6.10 Electromagnetic compatibility
   - 6.11 Regulatory requirements
7. [General construction requirements](#7-general-construction-requirements)
   - 7.1 Metal-enclosed cabinet
   - 7.2 Outdoor soft starter in hazardous areas
   - 7.3 Cooling
   - 7.4 Accessibility
   - 7.5 Wiring and terminal blocks
   - 7.6 Earthing
   - 7.7 Identification
   - 7.8 Painting
   - 7.9 Human-Machine Interface (HMI)
   - 7.10 Anti-condensation heating element
   - 7.11 Manufacturer's nameplate
8. [Inspection and testing](#8-inspection-and-testing)
   - 8.1 Factory Acceptance Tests
   - 8.2 On-site checks and tests
   - 8.3 Test and inspection report
   - 8.4 List of tests and inspections to be carried out
9. [Packaging and shipment](#9-packaging-and-shipment)
10. [Installation](#10-installation)
11. [Spare parts](#11-spare-parts)
    - 11.1 Commissioning and Start-Up
    - 11.2 Five and ten years operation
12. [Documentation](#12-documentation)
13. [Appendix 1: Documentation list](#13-appendix-1-documentation-list)
14. [Appendix 2: Schematic - Soft Starter in cabinet without bypass](#14-appendix-2-schematic---soft-starter-in-cabinet-without-bypass)
15. [Appendix 3: Schematic - Soft Starter in cabinet with bypass](#15-appendix-3-schematic---soft-starter-in-cabinet-with-bypass)
16. [Appendix 4: Data Sheets DS EP ELE 124](#16-appendix-4-data-sheets-ds-ep-ele-124)

---

## 1. Scope

This General Specification defines the minimum requirements for the design, manufacture, inspection and testing of low voltage soft starters.

Each soft starter is linked to a low voltage asynchronous motor to form a seamless and compatible assembly.

This specification shall be supplemented by a project specification and/or a data sheet defining the characteristics of each soft starter.

DC motor starters are outside the scope of this specification.

---

## 2. Reference documents

This document is adapted from TOTAL S.E. GS EP ELE 123 (Low Voltage Variable Speed Drive), transposed for LV Soft Starter equipment.

The reference documents listed below form an integral part of this General Specification.

### External Documents

Unless otherwise stipulated, the applicable version of these documents, including relevant appendices and addendums, is the latest revision published at the effective date of this document.

| Reference | Title |
|-----------|-------|
| EN 50495 | Safety devices required for the safe functioning of equipment with respect to explosion risks |
| European Directive 2011/65/EU | Directive on the restriction of the use of certain hazardous substances in electrical and electronic equipment |
| European Directive 2014/30/EU | Directive on the harmonisation of the laws of the Member States relating to electromagnetic compatibility |
| IEC 60079 (Parts 1; 2; 14) | Explosive atmospheres – Parts 1; 2; 14 |
| IEC 60204-1 | Safety of machinery – Electrical equipment of machines – Part 1: General requirements |
| IEC 60269-4 | Low-voltage fuses – Part 4: Supplementary requirements for fuse-links for the protection of semiconductor devices |
| IEC 60332-3-24 | Tests on electric and optical fibre cables under fire conditions – Part 3-24: Test for vertical flame spread of vertically-mounted bunched wires or cables – Category C |
| IEC 60445 | Basic and safety principles for man-machine interface, marking and identification – Identification of equipment terminals, conductor terminations and conductors |
| IEC 60529 | Degrees of protection provided by enclosures (IP Code) |
| IEC 60947-4-2 | Low-voltage switchgear and controlgear – Part 4-2: Contactors and motor-starters – AC semiconductor motor controllers and starters |
| IEC 62262 | Degrees of protection provided by enclosures for electrical equipment against external mechanical impacts (IK code) |
| IEC TS 60034-25 | Rotating electrical machines – Part 25: AC electrical machines used in power drive systems – Application guide |
| ISO 4628-3 | Paints and varnishes – Evaluation of degradation of coatings – Part 3: Assessment of degree of rusting |
| ISO 12944-2 | Paints and varnishes – Corrosion protection of steel structures by protective paint systems – Part 2: Classification of environments |

---

## 3. Applicability

This specification is applicable for all soft starters installed in cabinet, which can be installed:

- Offshore, coastal area or onshore,
- Safe or hazardous areas,
- Outdoor or indoor.

For each case, the specific requirements and location will be defined in the relevant data sheet.

---

## 4. Definitions of terms

For the purpose of this document, the following terms and definitions apply:

| Term | Definition |
|------|-----------|
| Company | Any entity of the TOTAL Group mentioned in the contract or the order. |
| Construction Contractor | The person or legal entity responsible for installing the equipment or a set of equipment covered by this specification. |
| Engineering Contractor | The person or legal entity responsible for performing the engineering services to procure the equipment covered by this specification. |
| Manufacturer | The person or legal entity responsible for manufacturing and/or supplying all or part of the equipment covered by this specification. |
| DC | Direct Current |
| EMC | ElectroMagnetic Compatibility |
| ESD | Emergency ShutDown |
| HMI | Human Machine Interface |
| IT system | Isolated neutral |
| LV | Low Voltage |
| PTC | Positive Temperature Coefficient |
| SIL | Safety Integrated Level |
| SS | Soft Starter |
| TNS | Neutral Earthed System and segregated |
| UPS | Unit Power System |

---

## 5. Scope of supply

The scope of supply is defined in the Requisition document attached in the Purchase Order and shall contain as a minimum:

- All documents listed in the chapter 12.
- One or several soft starters fully equipped and tested in accordance to the content required into this document, project particular specification and project data sheets (See Appendix 4 – DS EP ELE 124 filled up with project requirements).

---

## 6. Design

### 6.1 Service conditions

The equipment shall be designed to operate in an industrial environment.

Soft starters and all associated equipment shall be suitable for the specified place of installation.

#### 6.1.1 Installation inside electrical rooms

Unless otherwise specified, indoor electrical equipment shall be able to operate without damage or derating of performance as long as room temperature does not exceed 40°C.

The room's humidity level shall be defined in the project specification or data sheet.

#### 6.1.2 Installation outside electrical rooms

Outdoor electrical equipment shall be designed to operate continuously in environmental conditions as defined in the project specification or data sheet.

#### 6.1.3 Service life, life cycle and maintenance frequency

The Manufacturer shall guarantee a service life of 20 years, integrating the serial manufacturing period and follow up service (software and spare parts).

The Manufacturer shall guarantee operation of the equipment for a period of 6 years without needing any maintenance that entails shutting it down.

### 6.2 Definition of the equipment

The installation includes:

- A drawer or withdrawable circuit breaker located in an LV switchboard according to schematic diagram provided by Company or Engineering Contractor (outside the Manufacturer's scope).

- A cabinet containing the soft starter unit, with the power and command control circuits according to schematic diagrams provided by Company or Engineering Contractor.

- A by-pass system (internal or external), if requested by Company in the project particular specification or/and data sheet. The by-pass system shall allow direct on line running of the motor at full speed after the starting sequence is completed. The by-pass contactor shall be rated for continuous duty.

### 6.3 System voltage

#### 6.3.1 Voltages and neutral earthing

The soft starter shall be designed to start and control a low voltage asynchronous motor.

Unless otherwise specified in Project particular specification and/or data sheet, the voltages and neutral earthing system provided by the Company for electrical equipment will be:

- Main power supply: 690 V, 480 V or 400 V, 50 or 60 Hz – 3 phases – 3 wires – IT system (earthed via high impedance) or TNS.

- UPS distribution: 400 V / 230 VAC – IT system or TNS.

- DC distribution: 24 VDC, 48 VDC, 110 or 125 VDC unearthed.

Use of voltage levels and/or frequencies not herein recommended is subject to written Company approval.

Any other voltage required (control circuit, safety control voltage, etc.) shall be generated by the soft starter or supplied by the Manufacturer from UPS or DC distribution provided by Company.

The voltage converter provided by Manufacturer if any, shall comply with EMC requirements.

#### 6.3.2 Electrical system variations

Unless otherwise specified, electrical equipment shall operate satisfactorily with the following simultaneous variations, from their nominal value, when measured at the consumer input terminals.

**Voltage:**
- Steady state variations: ±10%,
- Transient variations: +20%, -20%, Recovery within 1.5 seconds.

**Frequency:**
- Steady state variations: ±5%,
- Transient variations: ±10% Recovery time: within 5 seconds.

### 6.4 Technical requirements

The soft starter and its motor shall be sized to ensure permanent service at full load under the conditions of the present general specification completed by the particular specification.

The soft starter and motor shall form an assembly of compatible equipment, suited to the starting torque requirements of the driven machine, from start-up to full speed.

The Manufacturer shall verify that the upstream protection and switching device is compatible with the technical characteristics of the soft starter.

Soft starters shall be protected by fuses as per IEC 60269-4 or current limiting circuit breaker.

The current-limiting fuses or circuit breaker shall be selected and sized following the soft starter Manufacturer's instructions.

The degree of protection of equipment shall be at least IP 21 for indoor cabinet and IP 55 for outdoor, as per IEC 60529.

The soft starter Manufacturer shall coordinate with motor Manufacturer for the appropriate choice of motor and soft starter.

The interface parameters and interactions between the motor and the soft starter, including installation guidance, shall meet the requirements of IEC TS 60034-25.

The soft starter shall comply with IEC 60947-4-2 requirements.

Unless otherwise specified, soft starters shall be designed for pollution degree 2 as a minimum.

Equipment weighing more than 25 kg shall be fitted with lifting rings.

In addition, the supporting floor surface under the soft starter cabinet shall be of non-flammable material.

### 6.5 Performance requirements

The soft starter equipment shall satisfy the following requirements:

- Remote start/stop,
- All interfaces as defined in the data-sheets and the typical schematics in appendixes,
- Voltage ramp soft starting with adjustable starting voltage and ramp time,
- Current limiting soft starting capability,
- Adjustable acceleration ramp time from 1.5 to 30 seconds, unless otherwise stipulated in the project specification,
- Adjustable deceleration (soft stop) ramp time,
- Starting current limitation capability (adjustable, typically 2 to 4 × FLA),
- A minimum power factor of 0.9 for the soft starter-motor assembly at full load,
- Motor starting torque suited to the driven machine load torque requirements.

The soft starter shall be capable of performing the specified number of starts per hour as defined in the project data sheet.

The Manufacturer shall specify the limit values for admissible voltage dips during starting.

### 6.6 Power cables

The type and length of cable between the motor and the soft starter shall be stipulated in the data sheet.

The manufacturer shall provide the instructions manual for cabling, screening and grounding of power cables.

### 6.7 Temperature sensors

Motors associated with soft starters are fitted with 1 set of 3 PTC sensors in series, placed in the stator windings.

When the sensor exceeds its temperature threshold, the safety function of the soft starter shall shutdown the motor.

For soft starter driven motor installed within potentially hazardous areas, the motor/soft starter association shall comply with the requirements of IEC 60079-14 and safety function of the soft starter certified ATEX as per EN 50495.

### 6.8 Protection devices and information

The protection system shall be electronic and have a dialogue interface capable, in the event of system faults, of providing sufficiently detailed information for trained personnel to repair the soft starter equipment.

For process ESD (Emergency shutdown) purpose, soft starters shall be fitted with a stop function category 0 as per IEC 60204-1 and SIL 2 safety integrated level, if requested by risk analysis.

The following minimum protection functions shall be provided/displayed:

**Motor:**
| Protection | Trip |
|-----------|------|
| Short circuit | X |
| Overload | X |
| Stator overheating (PTC sensor) | X |
| Unbalance current | X |
| Earth fault | X |
| Locked rotor | X |
| Excessive number of starts | X |

**Soft Starter:**
| Protection | Trip |
|-----------|------|
| Line over voltage | X |
| Thyristor (SCR) over temperature | X |
| Thyristor (SCR) short circuit | X |
| Thyristor (SCR) open circuit | X |
| Heatsink over temperature | X |
| Cooling fault | X |
| Emergency stop | X |
| Loss of control voltage | X |
| Phase loss / phase reversal | X |

A general trip contact shall be connected to terminals for immediate action on the upstream breaking device.

The following minimum information shall be available on the front panel face of the soft starter cabinet:

- Motor current,
- Alarms (overload, etc.),
- Trip causes,
- Input/Output status,
- Software version (through HMI display or Maintenance PC interface),
- Indication lights using LED for the following signals:
  - Ready for operation,
  - Starting (ramping),
  - Running (at full speed / bypassed),
  - Soft starter alarm,
  - Soft starter trip.

A 4-20 mA signal shall be available at terminals so that motor current can be displayed on a remote panel.

The loss of the power supply shall not prevent the reading of alarms on dialogue interface.

The communicating interface between soft starter and electrical control system shall be defined in the project particular specification or data sheet.

### 6.9 Noise levels

Unless otherwise specified, the noise level generated by the equipment at a distance of one meter in all directions shall not exceed 80 dBA for all loads from zero to rated load.

### 6.10 Electromagnetic compatibility

The soft starter shall meet the immunity levels of IEC 60947-4-2.

The Manufacturer shall provide recommendations for the installation and connection of the soft starter equipment, to obtain a complete assembly compliant with EMC requirements.

### 6.11 Regulatory requirements

For European projects, the equipment supplied shall bear the "CE" marking indicating compliance with European standards.

Soft starters to be installed within the European Union shall comply with European Directive 2014/30/EU related to Electromagnetic Compatibility and European Directive 2011/65/EU on the restriction of the use of certain hazardous substances in electrical and electronic equipment.

---

## 7. General construction requirements

### 7.1 Metal-enclosed cabinet

The soft starter shall be installed in one or more free-standing metal cabinets designed for indoor operation.

The equipment shall be arranged so as to provide access inside the cabinet without shutting down the soft starter.

Each cabinet shall be designed to allow front access for normal maintenance operations.

Removable side panels may be provided, but rear access should not be needed.

Access to the equipment shall be designed for ease of maintenance.

The thickness of the steel plates shall be sufficient to ensure excellent overall rigidity.

Each cabinet shall have a degree of protection of at least IK 08 as per standard IEC 62262 and a key-lockable handle for opening and closing it.

The key-locks will be defined in the particular specification.

Lifting rings shall be provided.

### 7.2 Outdoor soft starter in hazardous areas

Outdoor soft starters installed in potentially hazardous area shall be suitable certified category 2G with either Ex"d" or Ex "px" protection mode as per IEC 60079-1 or IEC 60079-2, respectively.

### 7.3 Cooling

Cooling by natural convection shall be preferred.

However, if forced ventilation is needed, the fans shall offer high reliability, a lifetime ≥ 55,000 hours and their operation be permanently monitored.

Indicator lights and alarm contacts shall be provided for fan faults and for clogged filters.

### 7.4 Accessibility

The location and grouping of the components and auxiliary equipment shall allow easy identification and easy front access for operation, maintenance and repair purposes.

Appropriate partitioning between the different functional units shall be provided, to allow adjustments and verifications to be carried out in total safety.

All exposed busbars and live equipment parts located inside the cabinet shall have at least IP 20 protection.

### 7.5 Wiring and terminal blocks

The wiring inside the cabinet shall be single-core with class 5 copper conductors.

The minimum cross-section of the wiring shall be 1.0 mm² (2.5 mm² for power cables), except for connections to printed circuit boards, where the minimum cross-section may be 0.75 mm².

The wiring shall be halogen-free and comply with category C of standard IEC 60332-3-24.

The wiring shall be held in place by insulating supports such as sleeves, ducting, plastic ties or strips and be arranged such as to prevent any mechanical damage.

Wiring between fixed parts and hinged doors shall be mechanically protected.

All components such as ducting, wiring, cable ties, etc. shall be made of flame-retardant materials.

Each wire shall be identified at each end as per the Manufacturer's wiring diagrams.

Terminal blocks shall be provided for all outside connections.

They shall be installed on standardized rails, be easily accessible and available with either spring or screw terminals.

Only one conductor shall be connected per terminal.

The cables shall enter from the bottom.

The terminals shall correspond to the cable type and cross-section determined in the data sheet or particular specification.

The manufacturer shall provide the instructions manual for cabling, screening and earthing of control cables.

### 7.6 Earthing

An Earthing dispatcher with a minimum cross-section between 16 and 35 mm² according to soft starter rated power, and a sufficient number of connections shall be installed near the cable entries to facilitate the bonding of cable armor and earthing conductors.

All exposed metallic parts, which might accidentally be energized, shall be connected to the earth bar.

The earth bar shall be linked to the main earth circuit via a connection terminal provided by the Manufacturer.

All earth connections shall be individual.

All removable metallic parts shall be connected to the frame and hinged doors earthed via flexible connections.

### 7.7 Identification

All external devices used for operation, measurement or indication shall be clearly identified by an indelible functional label, to facilitate identification by the operator.

All the components shall be identified by a tag in accordance with the identification system used by the Manufacturer, and marked on the diagrams and reference documents.

All indoor tags and labels shall be made from a corrosion resistant material, and indelibly marked (white dilophane or gravoply labels with black etching).

Identification by tag shall be installed with glue and plastic rivet.

All outdoor tags and labels shall be stainless steel etching.

Identification by tag shall be installed with stainless steel rivet.

The identification and marking of terminals, and general rules for the use of colours or alphanumeric notations to identify conductors, shall meet requirement of IEC 60445.

### 7.8 Painting

For indoor equipment, the surface treatment and protection of the steel plates shall comply with the Manufacturer's standard, but include cleaning, degreasing, and application of an anti-rust primer and a finishing coat, so as to provide effective protection against corrosion under the specified climatic and operating conditions.

Colour shall be of Manufacturer's standard, unless otherwise specified in the project specification.

For outdoor equipment, the painting system shall be, according to ISO 12944-2, category C4 Medium for onshore area and C5-M for offshore area.

The Manufacturer shall submit his coating system for protection against external corrosion for Company approval.

For outdoor applications, Manufacturer shall provide a warranty of 5 years – with a rusting degree Ri = 2, as per ISO 4628-3.

### 7.9 Human-Machine Interface (HMI)

The soft starter shall have an HMI on its front, for configuration purposes and to display the measurements and operating status.

If there is a fault, the alarm message describing the fault shall appear automatically on the display.

Soft starter Manufacturer shall provide software tools for programming and graphic representation of signals and alarms.

### 7.10 Anti-condensation heating element

If requested by Company in the data sheet, hygrostat controlled anti-condensation heating element, shall be supplied at 230 VAC – 50 or 60 Hz single phase (external power supply provided by Contractor).

### 7.11 Manufacturer's nameplate

A Manufacturer's nameplate shall be provided with each part of the equipment, showing the following information:

- Manufacturer's name and address,
- Manufacturer's identification reference,
- Rated input voltage,
- Rated motor power (kW),
- Rated current (A),
- Utilisation category (AC-53),
- Serial number and year of manufacture.

---

## 8. Inspection and testing

### 8.1 Factory Acceptance Tests

Each soft starter shall be tested for compliance with the specifications attached to the order, with standards, applicable regulations and Manufacturer documents.

As a minimum, the routine tests defined in IEC 60947-4-2 shall be performed.

The type test certificates, as per IEC 60947-4-2, shall be provided.

Unless otherwise specified, the factory tests shall be done in the presence of a Company representative with a minimum 2 weeks prior notice.

### 8.2 On-site checks and tests

After installation and connection have been completed by the Construction Contractor and unless otherwise specified in the data sheet, the Manufacturer shall assist Company in configuring, on-site testing and commissioning of the equipment.

### 8.3 Test and inspection report

The Manufacturer shall issue a complete report of the factory acceptance tests as defined in the applicable standards.

Inspection reports shall also be issued.

On-site tests shall also be recorded in a test report.

### 8.4 List of tests and inspections to be carried out

| Description of the test or inspection | Factory | On-site |
|---------------------------------------|---------|---------|
| Verification of compliance with the specifications of the order, standards and supplier documents | X | |
| Visual inspection | X | X |
| Routine tests as per IEC 60947-4-2 | X | |
| Functional tests of the soft starter coupled with the motor | | X |

---

## 9. Packaging and shipment

Special conditions regarding packaging, transportation and storage are stipulated in the documents "General Purchasing Conditions" or "Particular Purchasing Conditions".

After the tests and inspection, any traces of humidity shall be removed from the equipment before commencing packaging and shipment.

The equipment, accessories and consumables shall be clearly tagged to facilitate assembly and installation on site.

Any consumables, special tools or equipment required for assembly, commissioning and maintenance shall be shipped with the equipment.

A complete set of installation, operation and maintenance instructions shall be placed in the packages with the equipment.

Appropriate protection against mechanical damage and the effects of corrosion shall be applied for transportation and throughout storage on site.

---

## 10. Installation

The soft starter installation shall respect installation, operation, storage preservation and maintenance instructions/manuals supplied in the language of the country.

---

## 11. Spare parts

### 11.1 Commissioning and Start-Up

The Manufacturer shall include in its bid all the spare parts needed for testing and starting up the installation. Company reserves the right to request certain additional parts it considers critical.

The spare parts shall be delivered at the same time as the main equipment.

The list of spare parts is appended to the order.

The Manufacturer shall provide "Plug and Play" spare parts and/or all special tools to make spare parts "Plug and Play" on site (example for an electronic board: Software and Firmware, laptop, programming adapter and operating manual).

Packaged spare parts shall be clearly identified (storage).

### 11.2 Five and ten years operation

The Manufacturer shall include with its bid a price list of all the tools and spare parts required for five and ten years operation of the equipment.

The list of spare parts is appended to the order.

Packaged spare parts shall be clearly identified (storage).

---

## 12. Documentation

Refer to Appendix 1 for typical list.

---

## 13. Appendix 1: Documentation list

A separate specification shall list all the documents to be provided by the Manufacturer.

It shall include at least the documents below:

| Description | With the bid | After order |
|-------------|:---:|:---:|
| Deviation list to project specifications | X | |
| Completed data sheets | X | X |
| Description and guarantee of control hardware and software support during the expected lifetime of the soft starter | X | |
| Soft starter starting current-time curve superimposed to motor thermal limit curve | X | |
| Thermal dissipation expressed in watts | X | |
| Technical manual | | X |
| Wiring schematics | | X |
| General layout drawing, indicating the dimensions and weight | X | X |
| List of spare parts required for testing and commissioning | X | X |
| The price list of spare parts for two years of operation | X | |
| The installation, use and maintenance manuals | | X |
| Detailed wiring diagrams | | X |
| ATEX certificate as an equipment associated to control system of an ATEX motor located in hazardous area | X | X |
| List of equipment parts | | X |
| Type test certificates according to § 8.1 | X | X |
| Test and inspection reports | | X |

---

## 14. Appendix 2: Schematic – Soft Starter in cabinet without bypass

*(Schematic drawing to be provided)*

---

## 15. Appendix 3: Schematic – Soft Starter in cabinet with bypass

*(Schematic drawing to be provided)*

---

## 16. Appendix 4: Data Sheets DS EP ELE 124

*(Data sheets to be provided)*

---

> *This document is the property of TOTAL S.E., it contains confidential information which may not be disclosed to any third party, reproduced, stored or transmitted without the prior written consent of TOTAL S.E.*
> *The information contained in this document does not substitute for applicable laws and regulations.*
