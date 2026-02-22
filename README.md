# One‑Compartment Oral Absorption – Analytical Solution (MATLAB)

This project simulates plasma concentration after an oral dose using the closed‑form analytical solution for a one‑compartment pharmacokinetic model with first‑order absorption. The script computes concentration at each time point directly from the Bateman equation, eliminating the need for numerical ODE solvers. Results are displayed on both linear and semi‑log scales.

## What I Built

- **One‑compartment PK model** with first‑order elimination and first‑order absorption.
- **Oral dose**: dose `D` administered at time zero.
- **Analytical solution** (Bateman equation):  
  `Cp(t) = (D * ka / (V * (ka - CL/V))) * (exp(-(CL/V)*t) - exp(-ka * t))`  
  (with appropriate handling when `ka = CL/V` – here `ka` and `CL/V` are distinct)
- **Implementation**: Vectorized calculation for all time points in one line.
- **Visualization**:
  - Linear plot (left subplot) – shows the absorption phase and elimination.
  - Semi‑log plot (right subplot) – reveals the log‑linear terminal phase.
<img width="560" height="338" alt="image" src="https://github.com/user-attachments/assets/f855d47e-647f-4599-a7d6-f1ba6e37e8b6" />


## Skills Demonstrated

- MATLAB programming (vectorized operations, subplots)
- Pharmacokinetic modeling (oral absorption, Bateman equation)
- Analytical derivation and implementation of PK equations
- Data visualization (linear and semi‑log scales, labeling, grid)

## How to Run

1. Open the script (e.g., `OneComp_Oral_Analytical.m`) in MATLAB.
2. Click **Run** or type the filename in the Command Window.
3. Modify parameters (`D`, `CL`, `V`, `ka`) at the top of the script to explore different scenarios.

The script generates one figure with two subplots: linear and semi‑log.


- `OneComp_Oral_Analytical.m` – main MATLAB script.

