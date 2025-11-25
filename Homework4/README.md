# Discrete Elastic Rod — Homework 4

This repository contains my full implementation of Homework 4 using the Discrete Elastic Rod (DER) model with implicit time integration.  
The project is divided into three parts.

---

## Part 1 — Dynamic Response

Simulates the dynamic behavior of a helical rod under a characteristic load.

Outputs:
- End-node displacement vs. time  
- Automatically detected steady-state displacement  
- 3D rod snapshots at several time steps

---

## Part 2 — Force–Displacement Curve (Logspace Sweep)

Force sweep from **0.01 F_char** to **0.5 F_char** using logarithmic spacing.  
Steady state is detected using a small-variation criterion.

Outputs:
- Force vs. displacement plot
- Log–log scaling plot
- Fitted stiffness value

---

## Part 3 — Diameter Sweep vs Textbook Prediction

Tests the classic spring stiffness formula:

├── part1/ # Part 1 code
├── part2/ # Part 2 code
├── part3/ # Part 3 code
├── report/ # Final PDF report
└── README.md


---

## How to Run

Run all simulations:

