# Buck Converter Modeling in Simulink

## Overview

This project presents the modeling, simulation, and validation of a DC-DC
Buck converter using both switched and averaged representations in Simulink.

The main objective is to demonstrate the equivalence between the switched
and averaged models under continuous conduction mode (CCM), and to validate
the suitability of the averaged model for control-oriented design and
system-level analysis.

The project follows MathWorks modeling best practices for power electronics
systems.

---

## Repository Structure

buck-converter/
│
├── models/
│ ├── buck_switched.slx
│ ├── buck_averaged.slx
│
├── scripts/
│ ├── buck_switched_vs_averaged.mlx
│
├── docs/
│ └── buck_switched_vs_averaged.pdf
│ ├── buck_switched_vs_averaged.docx

│
└── README.md


---

## Models Description

### Switched Model

The switched model is a detailed time-domain representation of the Buck
converter including the power switch and diode. This model captures
high-frequency switching behavior, voltage ripple, and inductor current
dynamics.

### Averaged Model

The averaged model is a continuous-time representation obtained by averaging
the converter dynamics over one switching period. This approach eliminates
switching ripple while preserving the mean system behavior, making it
well-suited for control design and rapid simulation.

---

## How to Run the Project

1. Open MATLAB and navigate to the project root directory.
2. Open the Live Script:

3. Run all sections sequentially.
4. Simulation results and comparison figures will be generated automatically.

---

## Key Results

- The averaged model accurately reproduces the mean output voltage of the
switched model.
- High-frequency switching ripple is removed in the averaged representation.
- The averaged model is validated for control-oriented modeling under CCM
operation.

---

## Requirements

- MATLAB R2022b or later
- Simulink
- Simscape Electrical (optional, depending on model implementation)

---

## Author

Luis Gaona  
Power Electronics Engineer

