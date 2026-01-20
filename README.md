# PI Game: Optimal Order Quantity Estimation for a Bakery Chain

**Authors:** Pooya Mers, Dinh Duy Phan, Rongyue Hua, Dan Ni Zhao, Zhenhua Yuan  
**Date:** June 2024  
**Course:** Academic Skills and Probability Inference  

## Project Summary  
This project applies the classical **Newsvendor Problem** to determine optimal daily production quantities for a bakery chain in Vilnius, Lithuania. The goal is to balance the cost of overstocking (waste) and understocking (lost sales) by estimating the **optimal order quantity** using both **parametric** and **non‑parametric** approaches.  
The analysis combines theoretical modeling, simulation studies, and real‑world demand data from four bakery locations.

## Problem Statement  
Perishable goods such as bread must be produced in the right quantity: too much leads to waste, too little leads to lost revenue.  
The bakery chain wants to understand:

1. **How to estimate the optimal order quantity \(Q^*\)** under different assumptions about demand.  
2. **How parametric and non‑parametric estimators compare** in accuracy and robustness.  
3. **How price adjustments should be made** when production costs increase.

## Approach  
- Developed an extended profit function incorporating selling price, production cost, clearance price, and shipping cost.  
- Derived the optimal order quantity  
  

\[
  Q^* = F^{-1}\left(\frac{c_u}{c_o + c_u}\right)
  \]

  
  where \(c_u\) and \(c_o\) represent underage and overage costs.  
- Compared **parametric (Normal / Log‑normal)** and **non‑parametric (order‑statistic)** estimators using **Monte Carlo simulations** across multiple sample sizes and service levels.  
- Conducted empirical analysis on four stores (Main Street A & B, Station A & B), including:  
  - descriptive statistics  
  - histograms and time‑series plots  
  - Jarque‑Bera tests for distributional fit  
- Computed **point estimates and 95% confidence intervals** for optimal quantities.  
- Modeled long‑run pricing decisions under a projected **25% cost increase**.

## Results  
- **Parametric estimation performs best** when the true demand is Normal, especially with small samples and high service levels.  
- **Non‑parametric estimation is more robust** when the distribution is unknown, skewed, or heavy‑tailed.  
- Empirical optimal quantities for the bakery chain:  
  - **Main Street A (Saturday):**  
    - Parametric: ~138 units  
    - Non‑parametric: ~139 units  
  - **Station B (Sunday):**  
    - Both methods: ~100 units  
- Price‑sensitivity analysis suggests that to maintain current profit levels under rising costs:  
  - **Main Street A:** increase price by ~21%  
  - **Station B:** increase price by ~18%

## Key Takeaways  
- The Newsvendor framework provides a practical and data‑driven method for optimizing production of perishable goods.  
- Parametric methods excel when distributional assumptions hold; non‑parametric methods offer flexibility when they do not.  
- Simulation studies are essential for understanding estimator behavior under different demand scenarios.  
- The bakery chain can use these insights to reduce waste, improve profitability, and plan price adjustments strategically.
