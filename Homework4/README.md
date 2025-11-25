# Homework 4 — Discrete Elastic Rod (DER)

This repository contains my implementation of Homework 4 for the Discrete Elastic Rod (DER) model.  
The project includes the full simulation code (Jupyter notebook) and the final written report (PDF).

---

## 📂 Files

### `Homework4_V4.ipynb`
- Main notebook containing the full implementation for all three parts:
  - **Part 1:** Dynamic response and steady-state detection  
  - **Part 2:** Force–displacement sweep (logspace) and stiffness fitting  
  - **Part 3:** Diameter sweep and comparison with the textbook formula  
- Includes all simulation code, plotting functions, and generated figures.

### `Homework4_ZHAO.pdf`
- Final compiled report for Homework 4.  
- Contains explanations, equations, figures, and analysis corresponding to all simulation results.

---

## ▶️ How to Run

1. Open the notebook:
   Homework4_V4.ipynb
3. Run all cells from top to bottom.
4. All figures and results (Part 1–3) will be generated automatically.

---

## 📝 Requirements
Python 3.9+
numpy
matplotlib


---

## 📄 Notes

- The notebook uses an implicit DER solver with stretch, bending, and twist terms.
- Part 2 uses **logarithmic force sweep** and automatic **steady-state detection**.
- Part 3 compares the simulated axial stiffness to the classical formula  
  `k = G d^4 / (8 N D^3)`.

---



