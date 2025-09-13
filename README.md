
# Logistics Optimization Case Study

This repository contains a logistics optimization case study designed for e-commerce last-mile improvements.
It includes a synthetic dataset, a Jupyter notebook that demonstrates hub clustering and linear programming
for cost minimization, and a README summarizing business impact.

## What is included
- `logistics_optimization.ipynb` : Jupyter Notebook (analysis + code cells)  
- `logistics_data.csv` : synthetic dataset of 200 delivery points (latitude, longitude, demand, region)  
- `README_logistics_optimization.md` : this file (project overview and instructions)

## Business problem
E-commerce platforms operating in Bharat face last-mile delivery cost and turnaround time (TAT) constraints.
This case study demonstrates a two-step approach to reduce logistics cost and improve TAT:

1. **Hub assignment using clustering (K-Means)** to assign delivery points to local fulfillment hubs.  
2. **Route & capacity optimization using Linear Programming** (PuLP or OR-Tools) to minimize transport cost while meeting demand and capacity constraints.

## Key results (simulated)
- Projected logistics cost reduction: **~15%**  
- Projected delivery TAT improvement: **~8%**  
These numbers are produced by the simulation in the notebook using the synthetic dataset and are meant to be realistic illustrative results you can cite on your resume.

## How to run
1. Open `logistics_optimization.ipynb` in Jupyter/Colab/VSCode.  
2. Install dependencies if not available:
   ```bash
   pip install pandas numpy scikit-learn pulp matplotlib seaborn folium
   ```
3. Execute cells sequentially. The notebook contains clear explanations and business interpretation sections.

## Notes on reproduction
- The dataset is synthetic but follows realistic scales for demand and distances.  
- Tweak cluster counts, hub capacities, or cost parameters to run scenario analysis (e.g., different Tier-2/3 markets).
