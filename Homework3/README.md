# Flexible Beam Simulation with PID Control

**Author:** Xiaoyang Zhao  
**Course:** 263F
**Date:** Nov 2025  

This project simulates a planar flexible beam under gravity using an implicit time-integration solver.  
A PID controller drives the beam’s midpoint along a circular trajectory while respecting workspace limits.

### Files
- `Homework3_1.ipynb` — Main Python/Colab implementation  
- `Homework3_ZHAO.pdf` — Final LaTeX report   

### How to Run
Open `Homework3_1.ipynb` in **Google Colab**  
Run all cells sequentially, and the script will automatically generate all result figures.

**RMS tracking error:** ~1 cm • **Solver:** Implicit Newton–Raphson • **Controller:** PI with saturation
