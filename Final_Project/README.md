README
Overview

This repository contains the final project for MAE 263F – Dynamics & Control of Structures.
The project simulates a flexible aerial ladder subjected to wind loading using an implicit Euler time integrator, including bending/stretching elasticity, Rayleigh damping, torsional base spring–damper, and distributed wind forces.

The final deliverables include:

Jupyter Notebook implementation (Project_263F.ipynb)

Final written report

Final presentation slides

Files

Project_263F.ipynb – Main simulation code implementing the dynamic ladder model. 

Project_263F.ipynb - Colab

263F_Final_Report.pdf – Complete written report.

263F_Final_Presentation.pptx – Presentation slides used in class.

Key Features

Cosserat-style beam discretization (bending + stretching)

Newton–Raphson implicit integration

Base rotational spring–damper model

Wind-induced distributed load using Reynolds-number-based drag model

Time history outputs + ladder shape snapshots

How to Run

Open the notebook Project_263F.ipynb in Jupyter / VSCode / Colab.

Run all cells to:

Execute simulations for multiple wind speeds (5 / 10 / 15 m/s)

Generate time-history plots

Plot ladder deformation snapshots

No additional dependencies are required beyond:

numpy
matplotlib

Author

Tony Zhao – UCLA Mechanical & Aerospace Engineering
Final project for MAE 263F.
