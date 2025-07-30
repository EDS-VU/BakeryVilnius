# PI Game: Optimal Order Quantity Estimation for a Bakery Chain

**Authors:** Pooya Mers, Dinh Duy Phan, Rongyue Hua, Dan Ni Zhao, Zhenhua Yuan  
**Date:** June 2024  
**Course:** Academic Skills and Probability Inference  

## Overview  
This project applies the classical **Newsvendor Problem** framework to optimize daily bread production for a bakery chain in Vilnius, Lithuania. By balancing the costs of overstocking (waste) and understocking (lost sales), we estimate the **optimal order quantity** using both **parametric** and **non‑parametric** methods.  

## Methodology  
1. **Theoretical Foundation**  
   - Formulated the profit function incorporating selling price, clearance price, production cost, and shipping cost.  
   - Derived the optimal order quantity \( Q^* = F^{-1}(\frac{c_u}{c_o + c_u}) \), where \(c_u\) and \(c_o\) are underage and overage costs.  
2. **Parametric vs. Non‑parametric Estimation**  
   - **Parametric:** assumes a known demand distribution (Normal/Log‑normal).  
   - **Non‑parametric:** uses order statistics without distributional assumptions.  
   - Compared using Monte Carlo simulations (500 iterations) across different sample sizes and service levels.  
3. **Empirical Analysis**  
   - Analyzed multi‑store demand data (Main Street A & B, Station A & B).  
   - Applied goodness‑of‑fit tests (Jarque‑Bera) to validate distributional assumptions.  
   - Computed **point estimates and confidence intervals** for \(Q^*\) using both methods.  
4. **Price Sensitivity**  
   - Modeled how to adjust prices to maintain profit levels given a 25% increase in costs.  
   - Estimated optimal price increases: **+21.0% for Main Street A** and **+18.2% for Station B**.

## Key Findings  
- If the true demand distribution is **Normal**, the **parametric estimator performs better**, especially at small sample sizes and high service levels.  
- If the distribution is unknown, skewed, or heavy‑tailed, **non‑parametric estimation is more robust**.  
- Empirical results for the bakery chain:  
  - **Main Street A (Saturday):** optimal order ≈ 138 units (parametric) vs 139 units (non‑parametric).  
  - **Station B (Sunday):** optimal order ≈ 100 units for both approaches.  
- Price‑increase analysis provides a clear guideline for maintaining profitability when costs rise.  


