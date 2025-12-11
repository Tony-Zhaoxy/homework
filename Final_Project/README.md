# MAE 263F Final Project – Flexible Ladder Simulation

This repository contains the final project for **MAE 263F Dynamics & Control of Structures**.  
It models a flexible aerial ladder subjected to wind loading using an **implicit Euler solver** with bending/stretching elasticity and a torsional base spring–damper system.

## Files
- **Project_263F.ipynb** – Main simulation code implementing the ladder dynamics.  
- **263F_Final_Report.pdf** – Full written report.  
- **263F_Final_Presentation.pptx** – Presentation slides.

## Highlights
- Cosserat-style beam discretization (stretching + bending)
- Newton–Raphson implicit integration
- Base rotational spring–damper model
- Distributed wind load based on Reynolds-number–dependent drag
- Time histories and deformation snapshots for different wind speeds

## How to Run
1. Open `Project_263F.ipynb` in Jupyter/VSCode/Colab.  
2. Run all cells to execute simulations (U = 5, 10, 15 m/s) and generate plots.

Dependencies:
```bash
numpy
matplotlib


Author

Xiaoyang Zhao – UCLA MAE
Shixuan Sun - UCLA MAE
Final project for MAE 263F.
