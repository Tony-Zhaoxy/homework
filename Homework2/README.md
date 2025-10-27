# MAE 263F – Homework 2  
**Author:** Xiaoyang Zhao  
**Date:** October 27 2025  
**Files:**  
- `Homework2_ZHAO.pdf` — Final report (Task 1 & Task 2)  
- `Homework2.ipynb` — Python code and results  

---

## 1 Project Description
This homework investigates the dynamic response and large-deflection behavior  
of a simply supported aluminum tube beam using an implicit Euler time-integration scheme.

### Task 1 – Implicit Simulation of Beam Deflection
- Beam length \(L = 1 \mathrm{m}\); outer/inner radii \(R = 0.013 \mathrm{m}, r = 0.011 \mathrm{m}\).  
- Load \(P = 2000 \mathrm{N}\) applied at \(x = 0.75 \mathrm{m}\).  
- \(N = 50\) nodes, \(\Delta t = 10^{-2}\,\mathrm{s}\).  
- Implicit Euler + Newton–Raphson iteration.  
- Steady deflection \(y_{max}^{sim} ≈ 0.038 \mathrm{m}\) matches Euler–Bernoulli theory.

### Task 2 – Load–Deflection and Nonlinear Behavior
- \(P \in [20, 20000] \mathrm{N}\) in 20 increments.  
- Load–deflection curve agrees with E–B theory for \(P<4000 \mathrm{N}\).  
- Deviation starts near \(P^* ≈ 7000 \mathrm{N}\) due to geometric stiffening.  
- Implicit solver remains stable throughout.

---

## 2 How to Run
1. Open `Homework2.ipynb` in Google Colab or Jupyter.  
2. Run all cells.  
3. Outputs:  
   - `Figure 1`: Time history of maximum deflection.  
   - `Figure 2`: Load–deflection curve (Task 2).  
4. Optional parameters for speed:  
   ```python
   Ps = np.linspace(20, 20000, 10)   # fewer load points  
   dt = 0.02                         # larger time step  
   C = np.eye(2*nv) * 1e-3           # light damping
