# OpenRefinery

# TECHNICAL SPECIFICATION: SMALL-SCALE PLASTIC-TO-FUEL PYROLYSIS SYSTEM
## Author: Gemini AI & Kazuto Kirigaya
## Subject: Waste-to-Energy (WTE) Conversion and Automated Fuel Fractionation

---

### 1. ABSTRACT
This paper outlines the theoretical and practical design of a decentralized pyrolysis plant capable of converting post-consumer plastic waste (primarily Polyethylene and Polypropylene) into high-quality liquid fuels. The system prioritizes high-purity yield through precise temperature control, oxygen exclusion via CO2 displacement, and automated mechanical separation of aqueous contaminants.

---

### 2. CORE PROCESS: THERMAL DECOMPOSITION (PYROLYSIS)
The fundamental principle is the "cracking" of long-chain hydrocarbons (polymers) into shorter chains (C5-C40) in the absence of oxygen.

#### 2.1 Atmospheric Control
To prevent combustion and explosion, the reactor must be void of Oxygen (O2). 
- Method: CO2 Displacement (Purging). 
- Execution: CO2 is injected at the reactor base. Due to its higher density compared to air, it displaces O2 through the top exhaust. A "Bubbler" (water-lock) at the end of the line prevents atmospheric backflow.

#### 2.2 Thermal Profile
The reactor must maintain an internal temperature of 350°C to 500°C. 
- Catalyst: Using Zeolite (Y-Zeolite) can lower the required activation energy and increase the octane rating of the resulting gasoline.

---

### 3. FRACTIONAL DISTILLATION AND CONDENSATION
Post-reactor vapors contain a mixture of gas, gasoline, kerosene, and diesel.

#### 3.1 The Three-Stage Condenser Array
To achieve tank-ready separation, the vapor stream is passed through three temperature-controlled zones:
1. Tank 1 (Heavy Oils/Diesel): Maintained at ~200°C. Heavy chains condense here.
2. Tank 2 (Kerosene): Maintained at ~120°C. Intermediate chains condense.
3. Tank 3 (Gasoline): Maintained at ~15°C via ice-water or active refrigeration. Light chains condense.

---

### 4. ADVANCED SEPARATION: THE DENSITY FLOAT (DICHTESCHWIMMER)
Water contamination is inevitable due to moisture in plastic waste. Since water is denser (1.0 g/cm³) than gasoline (~0.75 g/cm³), it settles at the bottom.

#### 4.1 Mechanical Water Discharge Valve
To automate water removal without electronic sensors, a "Density Float" is utilized.
- Component: A spherical float calibrated to a specific gravity of 0.85 g/cm³.
- Logic:
    - In Gasoline: The float is heavier than the fluid and sinks, sealing the bottom drain.
    - In Water: The float is lighter than the fluid and rises (buoyancy), opening the drain to let water escape.
    - Result: The system self-regulates, ejecting water while retaining fuel.

---

### 5. PURIFICATION AND ENGINE COMPATIBILITY
To protect internal combustion engines from "Plastic Wax" (paraffin residues) and micro-particles, a two-step post-processing is required:

1. Demister Pad: A stainless steel mesh at the reactor exit to catch liquid aerosols (wax) before they reach the condenser.
2. Active Adsorption: Passing the final gasoline through an Activated Carbon column to remove sulfur odors and color impurities.

---

### 6. MATHEMATICAL FOUNDATION (BUOYANCY)
The float design is governed by Archimedes' Principle:
$$F_b = \rho \cdot V \cdot g$$
Where:
- $F_b$ is the buoyant force.
- $\rho$ is the density of the fluid.
- $V$ is the volume of the displaced fluid.

For the float to operate correctly:
$$\rho_{gasoline} < \rho_{float} < \rho_{water}$$

---

### 7. CONCLUSION
While DIY plastic-to-fuel systems are theoretically capable of high efficiency, the safety of the engine depends on the precision of the fractionation and the removal of waxes. By integrating CO2 purging, fractional condensation, and density-based water separation, a high-purity fuel can be synthesized from waste materials, bringing us closer to a closed-loop energy cycle.
