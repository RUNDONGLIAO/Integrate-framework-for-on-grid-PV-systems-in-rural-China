# Integrate-framework-for-on-grid-PV-systems-in-rural-China
The framework provides demand-side, supply-side, and optimisation-side models for the design and optimisation of grid-connected PV systems for rural buildings in different climate zones in China.

# Usage guidelines
## Operation Steps
All code is divided into function definition code and use code, the code stored in the folder is the function definition code, do not change unless you what to check the errors.
### 1. EPW to CSV Conversion
Use `convert_EPW_to_CSV.py` to convert EPW weather file of selected location to CSV format.

### 2. Baseline Load Generation
Use `run_baselineload.py` to create annual baseline load data

### 3. DHW Simulation
Use `run_DHW_simulation.py` to simulate DHW profiles.

### 4. Gradient Coefficient Calculation
Use `calculate_graidents.py` to compute heating and cooling gradient coefficients for winter and summer

### 5. Demand Simulation
Use `run_demand_simulation.py` to simulate heating and cooling loads for the selected location.

### 6. Convert to electricity demand
Use `convertheatingcoolingtoelec.py` to convert heating and cooling loads to electricity demand.
Use `convertDHWtoelec.py` to convert DHW loads to electricity demand.

### 7. Load Profile Integration
Use `update_loadprofile.py` to merge heating and cooling electrical loads, baseline loads, and DHW electrical loads.

### 8. PV power generation simulation
Use `run_PV.py` to simulate 1kWp PV power generation for selected location.

### 9. System Optimization
Use `run_MILP.py` to run MILP for determining:
- Optimal PV system size
- Optimal battery storage capacity
- Optimal battery power
- Optimal pareto front of cost and CO2 

# Credits and contact
If you have any questions about the code please feel free contact [Rundong Liao](mailto:RundongLiao@outlook.com).

# Citation
If you use the code derived from it in academic work, please cite:

Rundong Liao, Massimiliano Manfren, Benedetto Nastasi (2025).
# License
The code is available under a BSD-3-Clause license.
