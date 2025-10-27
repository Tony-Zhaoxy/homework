# MAE 263F – Homework 2  
**Author:** Xiaoyang Zhao  
**Date:** October 27 2025  
**Files:**  
- `Homework2_ZHAO.pdf` — Final report (Task 1 & Task 2)  
- `Homework2.ipynb` — Python code and results  

---

## Task 1 – Implicit Simulation of Beam Deflection

- Beam length **L = 1 m**, outer/inner radii **R = 0.013 m**, **r = 0.011 m**.  
- Load **P = 2000 N** applied at **x = 0.75 m**.  
- **N = 50** nodes, **Δt = 1×10⁻² s**.  
- Implicit Euler + Newton–Raphson iteration.  
- Steady deflection **yₘₐₓ(sim) ≈ 0.038 m**, matching Euler–Bernoulli theory.

---

## Task 2 – Load–Deflection and Nonlinear Behavior

- Load range **P ∈ [20, 20000] N**, evaluated in 20 increments.  
- Load–deflection curve agrees with E–B theory for **P < 4000 N**.  
- Deviation starts near **P* ≈ 7000 N** due to geometric stiffening.  
- Implicit solver remains stable throughout.

---

### How to Run
1. Open `Homework2.ipynb`.  
2. Run all cells.  
3. Output figures:  
   - **Figure 1:** Time history of max deflection (Task 1)  
   - **Figure 2:** Load–deflection curve (Task 2)

Optional parameters for faster runtime:
```python
Ps = np.linspace(20, 20000, 10)  # fewer load points
dt = 0.02                        # larger time step
C = np.eye(2*nv)*1e-3            # small damping for faster convergence
