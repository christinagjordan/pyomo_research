# Data-Driven Parameter Estimation for a Population Balance Model

### Using `Pyomo.DAE` to Fit a Dynamic Model to Experimental Polystyrene Milling Data

---

### 📋 Project Overview

This project implements a dynamic population balance model (PBM) to describe the mechanochemical milling of polystyrene. The model, governed by a system of **50 Ordinary Differential Equations (ODEs)**, simulates the evolution of the polymer's molecular weight distribution over time.

The core of this work involved translating a complex physical system into a computational model using **Python** and the `Pyomo.DAE` library. I then leveraged this model to solve an inverse problem: estimating key unknown process parameters directly from a limited set of experimental lab data. This approach of inferring system behavior from data is a powerful technique in modern process systems engineering and data science.

---

### 🎯 Key Objectives

* **Model Development:** Translate the complex PBM differential equations into a robust and solvable `Pyomo.DAE` model.
* **Dynamic Simulation:** Accurately simulate the time-evolution of the polymer's mass distribution and validate it against experimental measurements.
* **Parameter Estimation:** Implement an inverse modeling framework to infer critical, unmeasurable system parameters from real-world experimental data.
* **Performance Optimization:** Re-engineer the model's formulation to dramatically reduce computational cost and solution time.

---

### 🚀 Results & Impact

* **Successful Parameter Inference:** The model successfully estimated key process parameters, demonstrating the ability to extract valuable insights from sparse experimental data.
* **High-Fidelity Simulation:** The final model accurately forecasted the molecular weight distribution at various time points, aligning with lab measurements.
* **80% Reduction in Computation Time:** Through strategic reformulation of the model and application of inverse modeling techniques, the simulation's computational efficiency was improved by **over 80%**, enabling faster iteration and analysis.



---

### 🛠️ Technology & Methodology

* **Core Libraries:** This project was developed in Python, primarily utilizing **`Pyomo`** for mathematical modeling and optimization, with its `pyomo.dae` extension for handling differential algebraic equations. **`Pandas`** was used for data manipulation and management.
* **Modeling Approach:** The population balance model tracks particle mass across 50 discrete size bins. The change in mass within each bin is described by a differential equation, creating a large, interconnected system. This system was then solved as an inverse problem to fit the model's predictions to the experimental data points.

---

### 🔬 Data Source & Acknowledgements

* All experimental data was collected by Yuchen Chang in the lab of Professor Carsten Sievers at the Georgia Institute of Technology. The experimental procedure is detailed in the following publication:
    * *Mechanistic Insights into the Mechanocatalytic Deconstruction of Polystyrene*, ACS Sustainable Chemistry & Engineering, 2023. [https://doi.org/10.1021/acssuschemeng.3c05296](https://doi.org/10.1021/acssuschemeng.3c05296)
* The inverse modeling approach is based on the methods detailed in:
    * *Solution of inverse problems for population balance models of granulation*, Powder Technology, 2011. [https://doi.org/10.1016/j.powtec.2010.12.019](https://doi.org/10.1016/j.powtec.2010.12.019)

---

### 👤 Contact

For any questions about this project, feel free to connect with me on LinkedIn!

**Christina Jordan** - [linkedin.com/in/christinagjordan](https://www.linkedin.com/in/christinagjordan)
