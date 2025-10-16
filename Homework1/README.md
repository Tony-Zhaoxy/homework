# Homework 1 – MAE 263F: Mechanics of Flexible Structures and Soft Robots
**Author:** Xiaoyang Zhao  
**Date:** October 16, 2025  

## Overview
This project implements and analyzes a 2D spring–mass network using the **implicit (backward) Euler** time integration method.  
Additional simulations using the **explicit Euler** and **Newmark–β** schemes are provided to compare numerical stability, damping, and energy conservation properties.

## Contents
- `Homework1.ipynb` — Main simulation notebook (Colab-compatible).  
- `nodes.txt`, `springs.txt` — Define network geometry and spring stiffness.  
- `Homework_ZHAO.pdf` — Full report including pseudocode, results, and discussion.  
- `figures/` — Simulation plots (network deformation and node displacements).

## How to Run
1. Open `Homework1.ipynb` in Google Colab or Jupyter Notebook.  
2. Run all cells sequentially to reproduce the simulation results.  
3. Plots of network deformation and node displacements will be displayed automatically.

## Summary of Results
- **Implicit Euler:** Stable for stiff networks but introduces numerical damping.  
- **Explicit Euler:** Simple but conditionally stable; energy grows with time.  
- **Newmark–β:** Provides tunable damping control and physically consistent oscillatory response.
