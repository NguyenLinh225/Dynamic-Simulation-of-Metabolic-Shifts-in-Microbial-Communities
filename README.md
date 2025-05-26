# install required packages
pip install cobra micom scipy matplotlib
# 🔬 Dynamic Simulation of Metabolic Shifts in Microbial Communities

This repository presents a computational framework to simulate the **dynamic metabolic interactions** between two microbial species (e.g., *Escherichia coli* and *Bacillus subtilis*) in co-culture over time using **dynamic Flux Balance Analysis (dFBA)**.

## 🎯 Project Goal

To model **metabolic competition and cooperation** between microbes in response to shared environmental resources (e.g., glucose) and by-products (e.g., acetate). The simulations incorporate **nutrient depletion, secretion, and uptake dynamics** using genome-scale metabolic models.

---

## 💡 Key Features

- ✅ **Dynamic Flux Balance Analysis (dFBA):** Track metabolite concentrations and fluxes over time using ODE integration and linear optimization.
- ✅ **Community Modeling:** Support for multiple organisms and interaction through shared environment.
- ✅ **Customizable Conditions:** Modify nutrient availability, uptake kinetics, or initial biomass.
- ✅ **Visualization:** Plot dynamic behavior of biomass, glucose/acetate levels, and fluxes.

---

## 🧰 Tools & Technologies

- [COBRApy](https://cobrapy.readthedocs.io/en/latest/): Core metabolic modeling
- [MICOM](https://micom-dev.github.io/): Community modeling of microbiomes
- `scipy.integrate`: Solving ODEs for metabolite concentrations
- `matplotlib`: Data visualization
- (Optional) KEGG/MetaCyc API: Reaction and pathway annotation

---

## 📁 Repository Structure

```bash
dFBA_Microbial_Community/
├── README.md                   # Project overview and instructions
├── notebooks/
│   └── dynamic_simulation.ipynb   # Interactive notebook: run and visualize dFBA
├── models/
│   └── ecoli.xml               # Genome-scale metabolic model for E. coli
│   └── bacillus.xml            # Genome-scale model for Bacillus subtilis
├── scripts/
│   └── dFBA.py                 # Core Python script for dFBA simulation
└── plots/
    └── biomass_plot.png        # Example output plots
